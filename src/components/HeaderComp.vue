<template>
  <header>
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="logo">
    </div>
    <nav>
      <ul>

        <li><a href="#">Characters</a></li>
        <li><a class="active" href="#">Comics</a></li>
        <li><a href="#">Movies</a></li>
        <li><a href="#">Tv</a></li>
        <li><a href="#">Games</a></li>
        <li><a href="#">Collectibles</a></li>
        <li><a href="#">Videos</a></li>
        <li><a href="#">Fans</a></li>
        <li><a href="#">News</a></li>
        <li><a href="#">Shop</a></li>

      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderComp'
}
</script>

<style lang="scss" scoped>
  header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    height: 120px;
    margin: auto;
    img{
      width: 80px;
    }
  }
  ul{
    display: flex;
    li{  
      margin: 0 0.5rem;
      a{
        text-transform: uppercase;
        &:hover,
        &.active{
          color: blue;
          border-bottom: 7px solid blue;
          padding-bottom: 45px;
        }
      }
    }
  }
  
</style>