<template>
  <div class="div1Sec2">
    <img src="../assets/fotoSecOne.png" class="fotoSecOne" alt="Temach">
      <div class="contenidoSec1">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat dolore obcaecati 
        libero voluptatem reiciendis voluptatum modi. Alias ut et nulla tempora? Tenetur aut 
        laborum laudantium pariatur molestiae ut, vitae nihil!</p>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.div1Sec2 {
  width: 100%;
  height: 100%;
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
  bottom: 20em; /*Alinea el título verticalmente en el centro */
  left: 50%; /*Alinea el título horizontalmente en el centro */
  transform: translate(-50%, -50%);  /*Centra el título*/
  z-index: 40;
  width: 40em;
}
</style>