<template>

  <div class="home-navbar">
    <div class="navbar-title">
        <img alt="DigDeeperLogo" id="DigDeeper-logo" src="../../assets/Pioche.png">
        <p>DigDeeper</p>
    </div>

    <div class="navbar-metamask">
        <button id="metamask-button" type="button" name="metaMask">
            install Metamask
        </button>
    </div>
  </div>
</template>

<script>
export default 
{
  name: 'HomeComponent'
}
</script>


<style scoped>
    @import '../../assets/styles/global/web/navbar.css';
    @import '../../assets/styles/global/mobile/navbar.css';
</style>

