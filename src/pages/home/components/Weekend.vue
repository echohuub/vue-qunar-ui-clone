<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl"/>
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
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
          title: '土楼的秘密',
          desc: '一座座神秘的建筑，一段段传奇的历史，在这里深刻体会历史留下的点点足迹，感受闽文化',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1509/b5/07bc81fc254ed6.jpg_r_640x214_8879c815.jpg'
        }, {
          id: '0002',
          title: '土楼的秘密',
          desc: '一座座神秘的建筑，一段段传奇的历史，在这里深刻体会历史留下的点点足迹，感受闽文化',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1509/b5/07bc81fc254ed6.jpg_r_640x214_8879c815.jpg'
        }, {
          id: '0003',
          title: '土楼的秘密',
          desc: '一座座神秘的建筑，一段段传奇的历史，在这里深刻体会历史留下的点点足迹，感受闽文化',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1509/b5/07bc81fc254ed6.jpg_r_640x214_8879c815.jpg'
        }]
      }
    }
  }
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    line-height .8rem
    background #eee
    text-indent .2rem

  .item-img-wrapper
    overflow hidden
    height 0
    padding-bottom 33.9%

    .item-img
      width 100%

  .item-info
    padding .1rem

    .item-title
      line-height .54rem
      font-size .32rem
      ellipsis()

    .item-desc
      line-height .4rem
      color #ccc
      ellipsis()
</style>
