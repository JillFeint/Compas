<template>
  <header class="headerGlobal">
    <!-- <div class="headerContainer"> -->
      <div class="logoHeader">
        <img class="logoHeaderImg" src="./assets/logo.png" alt="">
      </div>
      <div class="btnHeader">
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Chimbo</a></li>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Chimbo</a></li>
        </ul>
      </div>
    <!-- </div> -->
  </header>
  <section class="sec1">
    <div class="div-container">
      <portadaDeCompas/>
    </div>
  </section>
  <section class="sec2">
    <seccionOne/>
  </section>
</template>

<script>
// import carrucelCompas from "./components/carrucelDeVideos.vue";
import seccionOne from "./components/seccionOne.vue"
import portadaDeCompas from "./components/portadaCompas.vue"
export default{
components: {
  //   carrucelCompas,
  portadaDeCompas,
  seccionOne,
}
}
</script>

<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
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
.btnHeader ul {
  display: flex;
  gap: 10px;
  list-style: none;
  margin: 25px;
}
.btnHeader a {
  color: white;
  text-decoration: none;
}
.btnHeader a:hover {
  color: gray;
}
.div-container{
  background-color: rgb(0, 0, 0);
  height: 100%;
  flex-wrap: wrap;
}

@media (max-width: 768px) {
  .tituloUnico {
    font-size: 16.5px;
  }
}
/* Contenedo global */
</style>
