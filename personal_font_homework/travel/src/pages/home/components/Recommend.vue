<template>
  <div>
    <div class="recommend-title">  热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src=item.imgUrl />
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
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1704/c9/c936f3fccfc6d7eda3.img.jpg_200x200_46052773.jpg',
        title: '上海杜莎夫人蜡像馆',
        desc: '时尚专区上演T台大秀，华丽空间闪耀出亦梦亦幻的魔力。'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1607/7c/7cda8b6782dabd80b4.img.jpg_200x200_2039e660.jpg',
        title: '上海迪士尼乐园',
        desc: '拍照打卡圣地、与迪士尼朋友互动、逛吃好去处。'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1603/2f/2f171e53f017e8b390.water.jpg_200x200_9f77138f.jpg',
        title: '锦江乐园',
        desc: '锦江乐园作为上海老牌的景点，面对国际化的圣诞节，也主动出击，通过时尚的灯光装饰，增加喜庆的圣诞气氛，吸引年轻的群体来这里游玩'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1408/21/623fa85345d2ff700bfe1f9bf70697f3.jpg_200x200_81e37f5f.jpg',
        title: '外滩观光隧道',
        desc: '乘地铁沿647米长的色彩变换不断的隧道旅行，会让游客感觉如梦如幻。'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .recommend-title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-index: .2rem
  .item
    overflow: hidden
    display: flex
    height: 1.9rem
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      min-width: 0
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
      .item-button
        line-height: .44rem
        margin-top: .16rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
</style>
