<template>
<div class="globalContainerTwo">
  <div class="viewCenterTwo">
    <div><h1>Juan es gay</h1>
    <p>Programa una prueba de conducción hoy</p>
    </div>
    <div class="btnDown">
    <button class="btnOneOt">Prueba de conducción</button>
    <button class="btnTwoOt">Prueba de conducción</button>
    </div>
  </div>
</div>
</template>
<script>
</script>
<style scoped>
.globalContainerTwo{
  position: flex;
  width: 100vw;
  height: 100vh;
}
.viewCenterTwo{
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
  text-align: center;
  color: azure;
  padding-top: 5px;
  margin: 0;
  height: 80vh;
  width: 100vw;
}
.btnDown{
  display: flex;
  justify-content: center;
  gap: 10px;
  width: 100%;
}
/* El cuerpo */
.btnOneOt{
  background-color: rgb(41, 40, 40);
  color: rgb(206, 211, 211);
  font-size: 12px;
  cursor: pointer;
  padding: 10px 25px;
  border-radius: 5px;
  border: none;
  box-shadow: 0 0 2px rgba(144, 144, 144, 0.5);
}
.btnOneOt:hover{
  transform: translateY(-5px);
  color:rgb(255, 254, 254);
  background-color: rgb(135, 135, 135);
}
.btnTwoOt{
  background-color: azure;
  color: rgb(3, 3, 3);
  font-size: 12px;
  cursor: pointer;
  padding: 10px 25px;
  border-radius: 5px;
  border: none;
  box-shadow: 0 0 2px rgba(144, 144, 144, 0.5);
}
.btnTwoOt:hover{
  transform: translateY(-5px);
  color:rgb(255, 254, 254);
  background-color: rgb(135, 135, 135);
}
</style>
