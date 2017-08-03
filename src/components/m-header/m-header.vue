<template>
  <div class="m-header">
    <div class="icon"></div>
    <h1 class="text">Chicken Music</h1>
    <router-link tag="div" class="mine" to="/user">
      <i class="icon-mine"></i>
      </router-link>
  
  </div>
</template>

<script type="text/ecmascript-6">
  export default {}
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  
@import "~common/stylus/variable"
@import "~common/stylus/mixin"
  .m-header
    position: relative
    height: 44px
    color: #261d1d
    font-size: 0
    background:#ffdede
    .icon
      display: inline-block
      vertical-align: top
      margin-top: 6px
      width: 30px
      height: 32px
      margin-right: 9px
      margin-left: 30px
      bg-image('logo')
      background-size: 30px 32px
    .text
      display: inline-block
      vertical-align: top
      line-height: 44px
      font-size: $font-size-large
    .tab
      display: flex
      height: 30px
      width:200px
      position: absolute
      top:6px
      right: 200px
      line-height: 30px
      font-size: $font-size-large
      .tab-item
        flex: 1
        text-align: center
        margin-left:30px
        border:1px solid $color-theme 
        border-radius: 5px;
        .tab-link
          padding-bottom: 5px
          color: $color-text-l
        &.router-link-active
          .tab-link
            color: $color-theme
            background:#ccc
    .mine
      position: absolute
      top: 0
      right: 40px
      .icon-mine
        display: block
        padding: 12px
        font-size: 20px
        color: $color-theme
</style>