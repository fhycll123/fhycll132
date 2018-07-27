<template>
  <div>
    <div class="recommend-title">周末去哪儿</div>
    <ul class="">
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}<p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/fb/302620ed8350f8.jpg_r_640x214_25a07cb4.jpg',
        title: '橘子洲',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！毛嗲嗲的伟岸头像'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1507/95/bf81a1519705f0.jpg_r_640x214_b29fb0c8.jpg',
        title: '长沙生态动物园',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/89/b2beff9f28b0db.jpg_r_640x214_94143396.jpg',
        title: '湘江橘洲之星·长沙印象游轮游',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/ae/11f076c6cb7c47.jpg_r_640x214_6f643489.jpg',
        title: '宁乡龙泉漂流',
        desc: '一生必看的演出实至名归，很有特色，很有技巧！'
      }, {
        id: '0005',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1603/56/33894ef918e1a8.jpg_r_640x214_a9de6b4e.jpg',
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
    margin-bottom: .1rem
  .item-img-wrapper
    overflow: hidden
    height :0
    padding-bottom: 33.9%
    .item-img
      width : 100%
  .item-info
    padding : .1rem
    .item-title
      line-height: .54rem
      font-size : .28rem
      ellipsis()
    .item-desc
      line-height : .4rem
      font-size : .24rem
      color: #cccccc
      ellipsis()
</style>
