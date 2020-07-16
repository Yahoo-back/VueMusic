<template>
  <div class="my-header">
    <div class="icon"></div>
    <h1 class="text">Freedom Music</h1>

    <!-- 个人中心 -->
    <router-link to="/user" class="mine" tag="div">
      <i class="icon-mine"></i>
    </router-link>
  </div>
</template>

<script>
export default {
  data () {
    return {}
  }
}
</script>

<style lang="scss" scoped>
@import '~@/common/scss/const.scss';
@import '~@/common/scss/mymixin.scss';

.my-header {
  position: relative;
  height: 46px;
  text-align: center;
  color: $color-theme;
  font-size: 0;
  .icon {
    display: inline-block;
    vertical-align: top;
    margin-top: 6px;
    width: 34px;
    height: 34px;
    margin-right: 9px;
    @include bg-image('logo');
    background-image: url('../../../src/common/img/fm.png');
    background-size: 34px 34px;
  }
  .text {
    display: inline-block;
    vertical-align: top;
    line-height: 46px;
    font-size: $font-size-large;
  }
  .mine {
    position: absolute;
    top: 0;
    right: 0;
    .icon-mine {
      display: block;
      padding: 12px;
      font-size: 20px;
      color: $color-theme;
    }
  }
}
</style>
