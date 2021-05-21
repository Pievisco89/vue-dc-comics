<template>
  <main>
    <div class="container">
      <h4>Current Series</h4>
      <CardComp 
        v-for="(comic, index) in comics"
        :key="index"
        :card="comic"
      />
    </div>
    <span>Load more</span>
  </main>
</template>

<script>
import comics from '@/assets/data/dc-comics.js'
import CardComp from '@/components/CardComp.vue'


export default {
  name: 'MainComp',
  components:{
    CardComp
  },
  data(){
    return{
      comics
    }
  },
}

</script>

<style lang="scss" scoped>
  @import '@/assets/style/vars.scss';

  main{
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    background: black;
    color: white;
    padding: 0 0.8rem;
    & > .container{
      display: flex;
      flex-wrap: wrap;
      padding: 0.8rem 0;
    }
    h4{
      position: absolute;
      top: -5%;
      left: 10%;
      background-color: $f-color;
      padding: 1rem;
      font-size: 18px;
      font-weight: 700;
      text-transform: uppercase;
    }
    span{
      display: inline-block;
      background-color: $f-color;
      margin-bottom: 2rem;
      padding: 1rem 5rem;
      text-transform: uppercase;
      font-size: 16px;
      font-weight: 700;
      cursor: pointer;
    }
  }
</style>