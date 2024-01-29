<template>
<div class="videoBackground">
    <img src="../assets/fondoCar.png" class="videoPlay">
  Tu navegador no admite la etiqueta de video.
</div>
<div class="globalContainerOther">
  <div class="viewCenterScroll">
    <div><h1>Disfrute de mi negro</h1>
    <p>Programa una prueba de conducción hoy</p>
    </div>
    <div><button class="btnOneTwo">Prueba de conducción</button></div>
  </div>
</div>
</template>
<script>
</script>
<style scoped>
.globalContainerOther{
  width: 100vw;
  height: 100vh;
  position: flex;
}
/* El cuerpo */
.viewCenterScroll{
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
  text-align: center;
  color: azure;
  padding-top: 5px;
  margin: 0;
  height: 70vh;
  width: 100vw;
}
.btnOneTwo{
  background-color:rgb(206, 211, 211, 0,5);
  font-size: 15px;
  color: rgb(0, 0, 0);
  border: white 1px;
  cursor: pointer;
  border: 1px solid white;
  padding: 5px 25px;
  border-radius: 5px;
}
.btnOneTwo:hover{
  transform: translateY(-5px);
  color:rgb(255, 0, 0);
  background-color: azure;
}
</style>
