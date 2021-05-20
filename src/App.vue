<template>
  <div id="app">
    
    <HeaderComp />

    <MainComp />

  </div>
</template>

<script>
import HeaderComp from '@/components/HeaderComp.vue';
import MainComp from '@/components/MainComp.vue';
export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp
  }
}
</script>

<style lang="scss">
@import '@/assets/style/general.scss';
</style>
