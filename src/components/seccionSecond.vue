<template>
  <div :class="estilo">{{ contenido }}</div>
</template>

<script>
import axios from 'axios';

export default {
  data() {
    return {
      contenido: '',
      estilos: 'custom-div'
    }
  },
  mounted() {
    this.cargarContenido();
  },
  methods: {
    cargarContenido() {
      axios.get('/contenido.txt')
        .then(response => this.contenido = response.data)
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
.custom-div {
  background-color: rgb(8, 8, 8);
  padding: 10px;
  margin: 10px;
  border: 1px solid black;
  width: 300px;
  color: rgb(0, 227, 227);
}
</style>
