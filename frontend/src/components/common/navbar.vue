<template v-if="mobileView">

  <!-- MOBILE version -->
  <div class="home-header" v-if="mobileView">

    <!-- <div class="navbar-title">
        <p>DigDeeper</p>
    </div> -->

  
    <div class="header-menu" :class="{ oppenned }" @click="oppenned = !oppenned">
      <span class="cls"></span>

      <span>
        <ul class="sub-menu ">
          <li class="menu-link">
            <img src="../../assets/icons/home.svg" class="link-img">
            <a href="#about" title="about">Home</a>
          </li>
          <li class="menu-link">
            <img src="../../assets/icons/book.svg" class="link-img">
            <a href="#skills" title="skills">About</a>
          </li>
          <li class="menu-link">
            <img src="../../assets/icons/mining.svg" class="link-img">
            <a href="#jobs" title="jobs">Game</a>
          </li>
        </ul>
      </span>

      <span class="cls"></span>

    </div>

    <!-- <div class="header-menu">
      <img src="../../assets/icons/burgerMenu.svg" id="header-menu">
    </div> -->

  </div>
  
  <!-- <div class="home-navbar" v-if="mobileView">

    <div class="navbar-link">

      <div class="link-box">
        <img src="../../assets/icons/book.svg" class="link-img">
        <li class="link-li"><a href="#">about</a></li>
      </div>

      <div class="link-box">
        <img src="../../assets/icons/home.svg" class="link-img">
        <li class="link-li"><a href="#">home</a></li>
      </div>

      <div class="link-box">
        <img src="../../assets/icons/mining.svg" class="link-img">
        <li class="link-li"><a href="#">game</a></li>
      </div>

    </div>

  </div> -->
  

  <!-- DESKTOP version -->
  <div class="home-navbar" v-else>
    <div class="navbar-title">
        <p>DigDeeper</p>
    </div>

    <div class="navbar-link">
        <li class="link-li"><a href="#">home</a></li>
        <li class="link-li"><a href="#">about</a></li>
        <li class="link-li"><a href="#">enter game</a></li>
    </div>
    <div class="navbar-metamask">
      
    </div>
  </div>
</template>
<script>
import {showAt, hideAt} from 'vue-breakpoints'
export default 
{
  name: 'HomeComponent',
  components: { hideAt, showAt },
  data: () => ({
    oppenned: false,
    mobileView: false
  }),
  methods: {

    
    handleView() {
        this.mobileView = window.innerWidth <= 990;
    }
  },
  created() {
    this.handleView();
    window.addEventListener('resize', this.handleView);
  }
}
</script>


<style scoped>
    @import '../../assets/styles/global/web/navbar.css';
    @import '../../assets/styles/global/mobile/navbar.css';
</style>

