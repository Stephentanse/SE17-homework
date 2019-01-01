<template>
  <div class="icons">
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png'>
      </div>
      <p class='icon-desc'>热门景点</p>
    </div>
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png'>
      </div>
      <p class='icon-desc'>一日游</p>
    </div>
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png'>
      </div>
      <p class='icon-desc'>上海必游</p>
    </div>
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/76/eb88861d78fb9902.png'>
      </div>
      <p class='icon-desc'>动植物园</p>
    </div>
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1811/f6/e54fad3ea337b02.gif'>
      </div>
      <p class='icon-desc'>年终大促</p>
    </div>
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/ab/6f7d6e44963c9302.png'>
      </div>
      <p class='icon-desc'>泡温泉</p>
    </div>
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/b1/528a9e80403b8c02.png'>
      </div>
      <p class='icon-desc'>上海欢乐谷</p>
    </div>
    <div class="icon">
      <div class='icon-img'>
        <img class='icon-img-content' src='http://img1.qunarzz.com/piao/fusion/1803/47/c2b659e048b11602.png'>
      </div>
      <p class='icon-desc'>野生动物园</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl';
  .icons
    margin-top: .1rem
    overflow: hidden
    height: 0
    padding-bottom: 50%
    .icon
      position: relative
      overflow: hidden
      float: left
      width: 25%
      height: 0
      padding-bottom: 25%
      .icon-img
        position: absolute
        top: 0
        left: 0
        right: 0
        bottom: .44rem
        boxs-sizing: border-box
        padding: .1rem
        .icon-img-content
          display: block
          margin: 0 auto
          height: 100%
      .icon-desc
        position: absolute
        left: 0
        right: 0
        bottom: 0
        height: .44rem
        line-height: .44rem
        text-align: center
        color: $darkTextColor
</style>
