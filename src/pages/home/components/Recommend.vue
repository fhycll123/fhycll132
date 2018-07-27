<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul class="">
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{item.title}}<p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1710/f5/f575b0f463058f96a3.img.jpg_200x200_e772e5ef.jpg',
        title: '宁乡炭河古城',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/10/b7aa220089fa8054e6e012bafff63042.jpg_200x200_650160bf.jpg',
        title: '长沙生态动物园',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1610/8f/8f244e6a0ac12325a3.img.jpg_200x200_a6a1cd22.jpg',
        title: '湘江橘洲之星·长沙印象游轮游',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1507/32/d5e833a546367db1a238d1261ca254b8.water.jpg_200x200_3dc55b47.jpg',
        title: '宁乡龙泉漂流',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }, {
        id: '0005',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/a9/a9cd8c8550398407.water.jpg_200x200_4fb81eb4.jpg',
        title: '湖南大围山',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .recommend-title
    margin-top : .2rem
    line-height: .8rem
    background: #eeeeee
    text-indent: .2rem
  .item
    display:flex
    height : 1.9rem
    overflow: hidden
    .item-img
      width : 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex:1
      padding : .1rem
      min-width :0
      .item-title
        line-height: .54rem
        font-size : .32rem
        ellipsis()
      .item-desc
        line-height : .4rem
        color: #cccccc
        ellipsis()
      .item-button
        line-height : .44rem
        margin-top : .16rem
        background :#ff9300
        padding : 0 .2rem
        border-radius: .06rem
        color : #ffffff
</style>
