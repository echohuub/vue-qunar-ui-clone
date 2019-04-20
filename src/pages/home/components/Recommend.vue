<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl"/>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
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
          title: '厦门科技馆1',
          desc: '厦门科技馆厦门科技馆1',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1901/7c/7cb1cca588241d6ba3.img.jpg_200x200_297820fb.jpg'
        }, {
          id: '0002',
          title: '厦门科技馆2',
          desc: '厦门科技馆厦门科技馆2',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1901/7c/7cb1cca588241d6ba3.img.jpg_200x200_297820fb.jpg'
        }, {
          id: '0003',
          title: '厦门科技馆3',
          desc: '厦门科技馆厦门科技馆3',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1901/7c/7cb1cca588241d6ba3.img.jpg_200x200_297820fb.jpg'
        }, {
          id: '0004',
          title: '厦门科技馆4',
          desc: '厦门科技馆厦门科技馆4',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1901/7c/7cb1cca588241d6ba3.img.jpg_200x200_297820fb.jpg'
        }]
      }
    }
  }
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .recommend-title
    margin-top .2rem
    line-height .8rem
    background #eee
    text-indent .2rem

  .item
    display flex
    height 1.9rem
    overflow hidden

    .item-img
      width 1.7rem
      height 1.7rem
      padding .1rem

    .item-info
      flex 1
      padding .1rem
      min-width 0

      .item-title
        line-height .54rem
        font-size .32rem
        ellipsis()

      .item-desc
        line-height .4rem
        color #ccc
        ellipsis()

      .item-button
        line-height .44rem
        margin-top .16rem
        background #ff9300
        padding 0 .2rem
        border-radius .06rem
        color #fff
</style>
