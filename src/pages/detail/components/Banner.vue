<template>
  <div>
    <div class="banner" @click="handleBannerClick">
      <img class="banner-img" src="//img1.qunarzz.com/sight/p0/1710/f5/f575b0f463058f96a3.img.jpg_600x330_b4ab7f0d.jpg">
      <div class="banner-info">
        <div class="banner-title">宁乡炭河古城</div>
        <div class="banner-number"><span class="iconfont banner-icon">&#xe674;</span>66</div>
      </div>
    </div>
    <common-gallary
      :imgs="imgs"
      v-show="showGallary"
      @close="handleGallaryClose"
    ></common-gallary>
  </div>
</template>

<script>
import CommonGallary from 'common/gallary/Gallary'
export default {
  name: 'DetailBanner',
  data () {
    return {
      showGallary: false,
      imgs: ['http://img1.qunarzz.com/sight/p0/1803/f0/f0eb06680091d6c2a3.water.jpg_r_800x800_1fab1dbb.jpg', 'http://img1.qunarzz.com/sight/p0/1803/20/204ff797775012eea3.water.jpg_r_800x800_9f809f40.jpg']
    }
  },
  components: {
    CommonGallary
  },
  methods: {
    handleBannerClick () {
      this.showGallary = true
    },
    handleGallaryClose () {
      this.showGallary = false
    }
  }
}
</script>

<style lang="stylus" scoped>
  .banner
    position: relative
    overflow: hidden
    height: 0
    padding-bottom: 55%
    .banner-img
      width: 100%
    .banner-info
      display: flex
      position: absolute
      left: 0
      right: 0
      bottom: 0
      line-height: .6rem
      color: #fff
      background-image:linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, .8))
      .banner-title
        flex: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        padding: 0 .4rem
        line-height: .32rem
        height: .32rem
        margin-top: .14rem
        border-radius: .2rem
        background: rgba(0,0,0, .8)
        font-size: .24rem
        .banner-icon
          font-size: .24rem
</style>
