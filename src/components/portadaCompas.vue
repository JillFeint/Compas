<template>
  <div class="logoHeader1">
    <div class="overlay">
      <!-- Contenido del overlay -->
    </div>
  <img class="logoHeader11" src="../assets/WhatsApp Image 2024-02-04 at 12.51.05 PM.png" alt="">
    <div class="tituloUnico">
        <h1>Compas de Hierro Colombia</h1>
    </div>
    <div class="divParrafo">
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit, dolor ipsa! Ratione, 
        recusandae? Amet cupiditate, blanditiis asperiores, architecto itaque voluptates 
        mollitia accusamus ut consequuntur non ducimus natus aspernatur vitae necessitatibus?</p>
    </div>
    <div class="divButton">
      <button class="button">Mas informacion</button>
    </div>
  </div>
</template>

<script>
  export default {
}
</script>

<style>
.logoHeader1 {
  position: relative;
  display: flex;
  justify-content: center;
}
.logoHeader11 {
  display: block;
  width: 100%;
  max-width: 100%;
  height: auto;
  z-index: 1;
}
.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 10;
  background-color: rgba(0, 0, 0, 0.6);
  display: flex;
  justify-content: center;
  align-items: center;
}
/* Este es el h1 del titulo del header */
.tituloUnico{
position: absolute;
display: flex;
justify-content: center; 
align-items: center; 
color: rgb(255, 255, 255);
top: 20%; /* Alinea el título verticalmente en el centro */
left: 50%; /* Alinea el título horizontalmente en el centro */
transform: translate(-50%, -50%); /* Centra el título */
z-index: 20;
}
.divParrafo {
  position: absolute;
  top: 45%; /* Alinea el título verticalmente en el centro */
  left: 50%; /* Alinea el título horizontalmente en el centro */
  transform: translate(-50%, -50%); /* Centra el título */
  z-index: 40;
  color: rgb(255, 255, 255);
}
.divButton {
  position: absolute;
  top: 78%; /* Alinea el título verticalmente en el centro */
  left: 50%; /* Alinea el título horizontalmente en el centro */
  transform: translate(-50%, -50%); /* Centra el título */
  z-index: 30;
}
.button {
  padding: 1em 2em;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  letter-spacing: 5px;
  text-transform: uppercase;
  cursor: pointer;
  color: #ffffff;
  transition: all 1000ms;
  font-size: 13px;
  position: relative;
  overflow: hidden;
  outline: 2px solid #ff0000;
  background-color: #ff0000;
}
button:hover {
  color:beige;
  transform: scale(1.1);
  outline: 1px solid rgb(255, 255, 255);
  /* box-shadow: 2px 3px 6px -8px gray; */
}
button::before {
  content: "";
  position: absolute;
  left: -50px;
  top: 0;
  width: 0;
  height: 100%;
  background-color: black;
  transform: skewX(45deg);
  z-index: -1;
  transition: width 1000ms;
}
button:hover::before {
  width: 250%;
}
</style>