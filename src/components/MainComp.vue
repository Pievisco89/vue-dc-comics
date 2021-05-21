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
  mounted(){
    console.log(comics);
  }
}

</script>

<style lang="scss" scoped>
main{
  position: relative;
  text-align: center;
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
    background-color: #00a9d9;
    padding: 1rem;
    font-size: 16px;
    text-transform: uppercase;
  }
  span{
    display: inline-block;
    background-color: #00a9d9;
    margin-bottom: 2rem;
    padding: 1rem 5rem;
    text-transform: uppercase;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
  }
}
</style>