<template>
  <div>
    <Topbar />
    <Nuxt />
  </div>
</template>

<script>
import Topbar from '../components/Topbar.vue'

export default {
  components: {
    Topbar
  }
}
</script>

<style lang="scss">
@import '../styles/global.scss';
</style>
