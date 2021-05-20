<template>
  <div id="app">
    
    <HeaderComp />

    <MainComp />

    <SectionBlue />

    <FooterComp />

  </div>
</template>

<script>
import HeaderComp from '@/components/HeaderComp.vue';
import MainComp from '@/components/MainComp.vue';
import SectionBlue from '@/components/SectionBlue.vue';
import FooterComp from '@/components/FooterComp.vue';


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    SectionBlue,
    FooterComp
  }
}
</script>

<style lang="scss">
@import '@/assets/style/general.scss';
@import '@/assets/style/vars.scss';

</style>
