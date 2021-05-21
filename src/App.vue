<template>
  <div id="app">
    
    <HeaderComp />

    <JumbotronComp />

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
import JumbotronComp from '@/components/JumbotronComp.vue';


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    SectionBlue,
    FooterComp,
    JumbotronComp
  }
}
</script>

<style lang="scss">
@import '@/assets/style/general.scss';
@import '@/assets/style/vars.scss';
@import '@/assets/style/utilities.scss';

</style>
