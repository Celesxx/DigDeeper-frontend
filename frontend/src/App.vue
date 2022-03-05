<template>
  <div class="app">
    <router-view/>
  </div>
</template>

<style>
body {
  margin: 0px;
}



#app {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  width: 100vw;
  height: 100vh;

}

.app {
  width: 100%;
  height: 100%;
  background: url("./assets/Illustration144.png") no-repeat center fixed; 
  -webkit-background-size: cover; /* pour anciens Chrome et Safari */
  background-size: cover; /* version standardisée */
}

@media screen and (max-width: 540px)
{
    .app{ background: url("./assets/Illustration144.png") no-repeat center ; }
}

</style>
