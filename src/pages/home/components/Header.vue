<template>
  <div class="header">
    <div class="header-left">
        <div class="iconfont left-icon">&#xe624;</div>
    </div>
    <div class="header-input">
        <span class="iconfont">&#xe632;</span>
        输入城市/景点/游玩主题</div>
    <div class="header-right">
        {{city}}
        <span class="iconfont arrow-icon">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
@import '~@styles/varibles.styl';
.header
    display: flex
    line-height: .86rem
    background: $bgColor
    .header-left
        width: .64rem
        float: left
        .left-icon
            text-align: center
            font-size: .4rem
    .header-input
        flex: 1
        background: #fff
        border-radius: .1rem
        margin-top: .12rem
        margin-left: .2rem
        height: .64rem
        line-height: .64rem
        padding-left: .2rem
        color #ccc
    .header-right
        width: 1.24rem
        float: right
        text-align: center
        .arrow-icon
            font-size: .24rem
            margin-left: -0.4
</style>
