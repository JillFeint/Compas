<template>
    <div class="logoHeader1">
    <div class="overlay">
        <!-- Contenido del overlay -->
    </div>
    <img class="logoHeader11" src="../assets/WhatsApp Image 2024-02-04 at 12.51.05 PM.png" alt="">
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
    background-color: rgba(0, 0, 0, 0.8);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}
</style>
