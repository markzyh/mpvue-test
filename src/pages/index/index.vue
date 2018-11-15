<template>
  <div class="container">
    <banner-swiper :imgUrls="imgUrls" />  
    <nav-bar/>
  </div>
</template>

<script>
import bannerSwiper from '@/components/swiper/swiper'
import NavBar from '@/components/nav/nav'

export default {
  data () {
    return {
      motto: 'Hello World',
      userInfo: {},
      imgUrls: [
      'http://img02.tooopen.com/images/20150928/tooopen_sy_143912755726.jpg',
      'http://img06.tooopen.com/images/20160818/tooopen_sy_175866434296.jpg',
      'http://img06.tooopen.com/images/20160818/tooopen_sy_175833047715.jpg'
    ]
    }
  },

  components: {
   bannerSwiper,NavBar
  },

  methods: {
    bindViewTap () {
      const url = '../logs/main'
      wx.navigateTo({ url })
    },
    getUserInfo () {
      // 调用登录接口
      wx.login({
        success: () => {
          wx.getUserInfo({
            success: (res) => {
              this.userInfo = res.userInfo
            }
          })
        }
      })
    },
    clickHandle (msg, ev) {
      console.log('clickHandle:', msg, ev)
    }
  },

  created () {
    // 调用应用实例的方法获取全局数据
    this.getUserInfo()
  }
}
</script>

<style scoped>

</style>
