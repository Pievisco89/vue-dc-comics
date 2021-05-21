<template>
  <main>
    <div class="container">
      <CardComp 
        v-for="(comic, index) in comics"
        :key="index"
        :card="comic"
      />
    </div>
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
  background: black;
  color: white;
  & > .container{
    display: flex;
    flex-wrap: wrap;
    padding: 20px 0;
  }
}
</style>