<template>
  <footer>
    
    <div class="f-top">
      <div class="container">
        <section>
          <h3>Dc Comics</h3>
          <ul>
            <li>
              <a href="#">Characters</a>
            </li>
            <li>
              <a href="#">Comics</a>
            </li>
            <li>
              <a href="#">Movies</a>
            </li>
            <li>
              <a href="#">TV</a>
            </li>
            <li>
              <a href="#">Games</a>
            </li>
            <li>
              <a href="#">Videos</a>
            </li>
            <li>
              <a href="#">News</a>
            </li>
          </ul>

          <h3>Shop</h3>
          <ul>
            <li>
              <a href="#">Shop DC</a>
            </li>
            <li>
              <a href="#">Shop DC Collectibles</a>
            </li>
          </ul>
        </section>

        <section>
          <h3>Dc</h3>
          <ul>
            <li>
              <a href="#">Term Of Use</a>
            </li>
            <li>
              <a href="#">Privacy policy (New)</a>
            </li>
            <li>
              <a href="#">Ad Choices</a>
            </li>
            <li>
              <a href="#">Advertising</a>
            </li>
            <li>
              <a href="#">Subscriptions</a>
            </li>
            <li>
              <a href="#">Talent Workshops</a>
            </li>
            <li>
              <a href="#">CPSC Certificates</a>
            </li>
            <li>
              <a href="#">Rating</a>
            </li>
            <li>
              <a href="#">Shop Help</a>
            </li>
            <li>
              <a href="#">Contact Us</a>
            </li>
          </ul>
        </section>

        <section>
          <h3>Sites</h3>
        <ul>
          <li>
            <a href="#">DC</a>
          </li>
          <li>
            <a href="#">MAD Magazine</a>
          </li>
          <li>
            <a href="#">DC kids</a>
          </li>
          <li>
            <a href="#">DC Universe</a>
          </li>
          <li>
            <a href="#">DC Power Visa</a>
          </li>
        </ul>
        </section>

      </div>
    </div>
    <div class="f-bottom">
      <div class="container">
        <section>
          <button>Sign-up now!</button>

        </section>
        <section>
          <ul>
            <li>
              <a href="#">Follow us</a>
            </li>
            <li>
              <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
            </li>
            <li>
              <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
            </li>
            <li>
              <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
            </li>
            <li>
              <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
            </li>
            <li>
              <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
            </li>
          </ul>
        </section>
      </div>
      
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComp'
}
</script>

<style lang="scss" scoped>
@import '@/assets/style/vars.scss';

  footer{
    height: 480px;
    background-image: url('../assets/img/footer-bg.jpg'); 
    background-size: cover;
  }    
  .f-top{
    display: flex;
    align-items: center;
    height: 370px;
    margin: 0 auto;
    & > .container{
      background-image: url('../assets/img/dc-logo-bg.png');
      background-repeat: no-repeat;
      background-position: right;
    }
    
    section{
      float: left;
      margin-right: 3rem;
      h3{
        color: white;
        margin: 1.5rem 0;
      }
      li{
        margin-bottom: 0.5rem;
      }
      a{
        color: #959595;
      }
    }
  }
  .f-bottom{
    height: 110px;
    background-color: #303030;
    & > .container{
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100%;
    }
    button{
      background: none;
      border: 2px solid #00a9d9;
      color: white;
      text-transform: uppercase;
      padding: 10px 15px;
    }
    ul{
      display: flex;
      align-items: center;
      li{
        margin: 0.6rem;
      }
      a{
        color: $f-color;
        text-decoration: none;
        text-transform: uppercase;
      }
    }
  }
 
</style>