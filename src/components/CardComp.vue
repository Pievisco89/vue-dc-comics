<template>
  <div>
    <a href="#">
      <img :src="card.thumb" :alt="card.series">
      <h5> {{card.series}} </h5>
    </a>

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
    justify-content: center;
    flex-basis: calc(100% / 6);
    img{
      width: 180px;
      height: 185px;
      margin: 20px 0;
  }
    h5{
      width: 80%;
      text-transform: uppercase;
      color: white;
      margin-top: 0.5rem;
      font-size: 12px;
    }
  }
</style>