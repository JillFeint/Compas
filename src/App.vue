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
    <div class="logoHeader1">
      <img  class="logoHeader11" src="./assets/WhatsApp Image 2024-02-04 at 12.51.05 PM.png" alt="">
      <div class="overlay">
      <!-- <carrucelCompas/> -->
        <!-- Capa para la superposición oscura -->
      </div> 
    </div>
  </div>
  <div>
    <h1 class="tituloUnico">Compas de Hierro Colombia</h1>
  </div>
</template>

<script>
// import carrucelCompas from "./components/carrucelDeVideos.vue";

// export default{
//   components: {
//   carrucelCompas,
// }
// }
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
/* esto es provisional arreglar */
.logoHeader1{
  display: flex;
  justify-content: center;
  /* box-sizing: border-box; */
  width: 100%;
}
.logoHeader11{
  display: flex;
  justify-content: center;
  align-items: center;
  height: auto;
  width: 100%;
  z-index: 1;
}
.div-container{
  background-color: rgb(0, 0, 0);
  height: 100%;
  flex-wrap: wrap;
}
.overlay {
  position: absolute;
  justify-content: center;
  align-items: center;
  height: 30em;
  max-height:30em;
  width: 100%;
  max-width: 100%;  
  z-index: 10;
  background-color: rgba(209, 209, 209, 0.5);
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
