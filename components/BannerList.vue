<template>
  <div class="banner-list">
    <div class="banner-list-main">
      {{ number }}
    </div>
    <div class="banner-list-sub">
      {{ description }}
    </div>
  </div>
</template>
<script>
export default {
  props: {
    number: {
      type: String,
      default: '0'
    },
    description: {
      type: String,
      default: ' '
    }
  }
}
</script>
<style lang="scss" scoped>
.banner-list {
    display: flex;
    height: 83px;
    width: 230px;
    & > .banner-list-main {
        font-size: 48px;
        font-weight: 400;
        border-bottom: 1px solid #fff;
        width: 114px;
        display: flex;
        justify-content: center;
    }
    & > .banner-list-sub {
        font-size:14px ;
        font-weight: 400;
        padding-left:24px;
        padding-top:13px;
    }
}
</style>
