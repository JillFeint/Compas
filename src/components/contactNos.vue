<template>
  <div>
    <input type="text" v-model="nombre" placeholder="Nombre" />
    <input type="email" v-model="email" placeholder="Email" />
    <textarea v-model="mensaje" placeholder="Mensaje"></textarea>
    <button @click="enviarCorreo">Enviar</button>
    <button @click="limpiarCampos">Limpiar</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nombre: '',
      email: '',
      mensaje: ''
    };
  },
  methods: {
    enviarCorreo() {
      const correo = `mailto:destino@example.com?subject=Contacto&body=Nombre:${this.nombre}%0DEmail:${this.email}%0DMensaje:${this.mensaje}`;
      window.location.href = correo;
    },
    limpiarCampos() {
      this.nombre = '';
      this.email = '';
      this.mensaje = '';
    }
  }
};
</script>

<style scoped>
/* Estilos opcionales */
input,
textarea {
  margin-bottom: 10px;
}
</style>

