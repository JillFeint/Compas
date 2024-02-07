<template>
  <header class="headerGlobal">
    <!-- <div class="headerContainer"> -->
      <div class="logoHeader">
        <img class="logoHeaderImg" src="./assets/logo.png" alt="">
      </div>
      <div class="btnHeader">
        <ul>
          <li>inicio</li>
          <li>chimbo</li>
          <li>inicio</li>
          <li>chimbo</li>
        </ul>
      </div>
    <!-- </div> -->
  </header>
  
  <div class="div-container">
    <portadaDeCompas/>
  </div>
  <div>
    <h1 class="tituloUnico">Compas de Hierro Colombia</h1>
  </div>
</template>

<script>
// import carrucelCompas from "./components/carrucelDeVideos.vue";
import portadaDeCompas from "./components/portadaCompas.vue"
export default{
components: {
  //   carrucelCompas,
  portadaDeCompas,
}
}
</script>

<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  background-color: black;
}
/* Header */
.headerGlobal{
  display: flex;
  /* box-sizing: border-box; */
  background-color: black;
  /* background: url(./assets/header.png);
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover; */
  height: 5em;
  width: 100%;
  justify-content: center;
  align-items: center;
  justify-content: space-between;
}
.logoHeader{
  display: flex;
  box-sizing: border-box; 
}
.logoHeaderImg{
  width: 100em;
  height: auto;
  max-width: 50px;
  margin-left: 3em;
}
.btnHeader{
  color: white;
}
.btnHeader ul {
  display: flex;
  gap: 10px;
  list-style: none;
  margin: 25px;
}
.div-container{
  background-color: rgb(0, 0, 0);
  height: 100%;
  flex-wrap: wrap;
}
/* Este es el h1 del titulo del header */
.tituloUnico{
  display: flex;
  justify-content: center;
  color: rgb(255, 255, 255);
  box-sizing: border-box;
  margin-top: 2%;
}
@media (max-width: 768px) {
  .tituloUnico {
    font-size: 16.5px;
  }
}
/* Contenedo global */
</style>
