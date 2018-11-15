<template>
    <ul class="nav">
        <li>
            <img src="/static/images/spr.png" alt="">
            <div class="nav-text">
                <h3>医院简介</h3>
                <p>政府放心 百姓认可</p>
            </div>
        </li><li>
            <img src="/static/images/spr.png" alt="">
            <div class="nav-text">
                <h3>医院简介</h3>
                <p>政府放心 百姓认可</p>
            </div>
        </li><li>
            <img src="/static/images/spr.png" alt="">
            <div class="nav-text">
                <h3>医院简介</h3>
                <p>政府放心 百姓认可</p>
            </div>
        </li><li>
            <img src="/static/images/spr.png" alt="">
            <div class="nav-text">
                <h3>医院简介</h3>
                <p>政府放心 百姓认可</p>
            </div>
        </li>
    </ul>
</template>
<script>
    export default {

    data() {
      return {

      };
    },
    mounted() {}
  };
</script>
<style lang="scss">
.nav{
    overflow: hidden;
    li{
        overflow: hidden;
        width: 49.8%;
        float: left;
        padding:20rpx 0;
    }
    li:nth-child(1),li:nth-child(2){
        border-bottom: 1px solid #999;
    }
    li:nth-child(1),li:nth-child(3){
        border-right: 1px solid #999;
    }
    img{
    width: 60rpx;
    height: 60rpx;
    margin:0 20rpx;float: left;
}
}
.nav-text{
    float: left;
    h3{
        font-size: 36rpx;
    }
    p{
        font-size: 26rpx;
    }
}

</style>

