<template>
  <header>
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="logo">
    </div>
    <nav>
      <ul>

        <li
          v-for="(link, index) in links" 
          :key="index"
        >
          <a 
            :class="{'active' : link.current}"
            :href="link.url"
          >
            {{link.text}}
          </a>
        </li>

      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderComp',
  data(){
    return{
      links:[
        {
          text: 'Characters',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Comics',
          url: 'javascript:void(0)',
          current: true
        },
        {
          text: 'Movies',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Tv',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Games',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Collectibles',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Videos',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Fans',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'News',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Shop',
          url: 'javascript:void(0)',
          current: false
        },
      ]
    }
  }
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
        color: #464646;
        &:hover,
        &.active{
          color: #00a9d9;
          border-bottom: 7px solid #00a9d9;
          padding-bottom: 45px;
        }
      }
    }
  }
  
</style>