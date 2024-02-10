<template>
  <div class="div1Sec2Other">
    <img src="../assets/fotoSecOne.png" class="fotoSecOne" alt="Temach">
      <div class="contenidoSec1">
        {{ contenido2 }}
      </div>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  data() {
    return {
      contenido2: '',
      estilos: 'custom-div'
    }
  },
  mounted() {
    this.cargarContenido();
  },
  methods: {
    cargarContenido() {
      axios.get('/fotoDelTemach.txt')
        .then(response => this.contenido2 = response.data)
        .catch(error => console.error('Error al cargar el contenido:', error));
    }
  },
  computed: {
    estilo() {
      return ['custom-div', this.estilos];
    }
  }
}
</script>

<style>
.div1Sec2Other {
  width: 100%;
  height: 40.4em;
  background-color: rgb(0, 0, 0);
  padding-top: 3px;
}
.fotoSecOne {
  width: 100%;
  height: auto;
  z-index: -1;
}
.contenidoSec1 {
  position: relative;
  display: flex;
  justify-content: center; 
  align-items: center; 
  color: rgb(255, 255, 255);
  bottom: 20em;
  left: 50%; 
  transform: translate(-50%, -50%); 
  z-index: 40;
  width: 40em;
}
</style>