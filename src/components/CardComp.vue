<template>
  <div>
    
    <img :src="card.thumb" :alt="card.series">
    <h5> {{card.series}} </h5>

  </div>
</template>

<script>
  export default {
    name: 'CardComp',
    props:{
      card: Object
    }
  }
</script>

<style lang="scss" scoped>
  div{
    display: flex;
    flex-direction: column;
    flex-basis: calc(100% / 6);
    margin-top: 2rem;
    margin-bottom: 0.8rem;
    img{
      width: 180px;
      height: 185px;
      cursor: pointer;
    }
    h5{
      width: 80%;
      text-transform: uppercase;
      color: white;
      margin-top: 1rem;
      font-size: 12px;
      cursor: pointer;
    }
  }
</style>