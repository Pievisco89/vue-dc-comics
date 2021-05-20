<template>
  <section>
    
    <ul>
      <li>
        <a href="#">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
          <span>Digital Comics</span>
        </a>
        
      </li>
      <li>
        <a href="#">
          <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
          <span>Dc merchandise</span>
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
          <span>Subscription</span>
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator">
          <span>Comic shop locator</span>
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="dc-power-visa">
          <span>Dc power visa</span>
        </a>
      </li>
    </ul>
    
  </section>
</template>

<script>
export default {
  name: 'SectionBlue'
}
</script>

<style lang="scss" scoped>
section{
  height: 160px;
  background-color: #00a9d9;
  ul{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;

    li{
      margin: 0 2rem;
      a{
        display: flex;
        align-items: center;
        color: white;
        text-transform: uppercase;
        font-size: 0.8rem;
        img{
          width: 50px;
          margin: 0 0.6rem;
        }
      }
    }
  }
}

</style>