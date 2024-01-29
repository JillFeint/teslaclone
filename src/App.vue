<template>
  <div class="videoBackground">
  <video class="videoPlay" autoplay loop muted>
    <source src="./assets/bgCars.mp4" type="video/mp4">
    Tu navegador no admite la etiqueta de video.
  </video>
  </div>
  <div class="globalContainer">
    <header class="btnTop">
    <div class="logoContain">
      <img v-if="mostrarImagenNormal" class="logoHead" src="./assets/logo-tesla.png" alt="Imagen normal" @click="cambiarImagen">
      <img v-else class="logoHead" src="./assets/tesla.png" alt="Imagen cambiada" @click="cambiarImagen">
    </div>
    <div class="listAll">
      <ul class="listOne">
        <li class="liOne"><a href="#">Modelo S</a></li>
        <li class="liOne"><a href="#">Modelo 3</a></li>
        <li class="liOne"><a href="#">Modelo X</a></li>
        <li class="liOne"><a href="#">Modelo I</a></li>
        <li class="liOne"><a href="#">Powerwall</a></li>
        <li class="liOne"><a href="#">Carga</a></li>
      </ul>
    </div>
    <div>
      <ul class="listTwo">
        <li><a href="#">Soporte</a></li>
        <li><a href="#">Tienda</a></li>
        <li><a href="#">Cuenta</a></li>
        <li><a href="#">Menú</a></li>
      </ul>
    </div>
  </header>
  <div class="viewCenter">
    <div><h1>Disfrute de Tesla</h1>
    <p>Programa una prueba de conducción hoy</p>
    </div>
    <div><button class="btnOne">Prueba de conducción</button></div>
  </div>
  <br><br><br><br>
  <scrollerChange/>
  <scrollerChangeTwo/>
</div>
</template>
<script>
  import scrollerChange from './components/scrollerChange.vue'
  import scrollerChangeTwo from './components/scrollerChangeTwo.vue'

  export default {
    name: 'App',
    components: {
      scrollerChange,
      scrollerChangeTwo,
    },
    data() {
    return {
      mostrarImagenNormal: true
    };
    },
    methods: {
      cambiarImagen() {
      this.mostrarImagenNormal = !this.mostrarImagenNormal;
    }
    }
    }
</script>
<style>
body, html {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
#app {
  margin: 0;
  padding: 0;
  background-color: blueviolet;
}
.videoBackground{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
}
.videoPlay{
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.globalContainer{
  width: 100vw;
  height: 100vh;
  position: absolute;
}
/* Contenido del header */
.btnTop{
  display: flex;
  justify-content: space-between;
  align-content: center;
  z-index: 10;
}
.logoContain{
  display: flex;
  justify-content: center;
  align-content: center;
  margin: 0;
  padding: 20px;
}
.logoHead{
  height: auto;
  width: 200px;
  margin: 0;
  padding-left: 20px;
  transition: transform 0.3s ease-in-out;
}
.logoHead:hover{
  /* transform: translateX(5%) translateY(-5px); */
  /* transform: scale(1.2); */
}
.listAll{
  display: flex;
}
.listOne{
  display: flex;
  color: azure;
  list-style: none;
  padding: 0;
  gap: 15px;
}
.liOne{
  color: azure;
  padding-top: 12px;
  list-style: none;
  font-size: 15px;
}
.listTwo{
  list-style: none;
  color: rgb(208, 211, 211);
  display: flex;
  padding-right: 52px;
  gap: 15px;
  font-size: 12px;
} 
/* El cuerpo */
.viewCenter{
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
.btnOne{
  background: none;
  font-size: 15px;
  color: rgb(206, 211, 211);
  border: white 1px;
  cursor: pointer;
  border: 1px solid white;
  padding: 5px 25px;
  border-radius: 5px;
}
.btnOne:hover{
  transform: translateY(-5px);
  color:rgb(0, 0, 0);
  background-color: azure;
}
a {
  text-decoration: none;
  color: azure;
}
a:hover{
  color: rgb(110, 110, 110);
}
</style>
