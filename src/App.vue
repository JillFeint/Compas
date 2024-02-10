<template>
  <header class="headerGlobal">
    <!-- <div class="headerContainer"> -->
      <div class="logoHeader">
        <img class="logoHeaderImg" src="./assets/logo.png" alt="">
      </div>
      <div class="btnHeader">
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Directorio</a></li>
          <li><a href="#">Nose</a></li>
          <li><a href="#">Contacto</a></li>
        </ul>
      </div>
    <!-- </div> -->
  </header>
  <section class="sec1">
    <div class="div-container">
      <portadaDeCompas/>
      <seccionCarrucel/>
    </div>
  </section>
  <section class="sec2">
    <!-- <seccionSecond/>
    <contactNos/> Esto no es para este proyecto creo, no mover sin preguntarme Angel -->
    <seccionTwo/>
  </section>
  <footer class="footer"> &copy; Moncada, Ballestero & Jill Angel, Compas del codigo de hierro, 2024 Inc. All Rights Reserved.</footer>
</template>

<script>
// import carrucelCompas from "./components/carrucelDeVideos.vue";
import portadaDeCompas from "./components/portadaCompas.vue"
import seccionTwo from "./components/seccionTwo.vue"
// import seccionSecond from "./components/seccionSecond.vue"
import seccionCarrucel from "./components/seccionCarrucel.vue"
// import contactNos from "./components/contactNos.vue"
export default {
components: {
  //   carrucelCompas,
  portadaDeCompas,
  seccionTwo,
  // seccionSecond,
  seccionCarrucel,
  // contactNos,
},
data() {
    return {
      mostrarComponenteContacto: false
    };
  },
  methods: {
    mostrarContacto() {
      this.mostrarComponenteContacto = true;
    }
  },
};
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
.footer{
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #282525;  
  height: 2em;
  color: white;
}
</style>
