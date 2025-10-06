<template>
  <div id="app">
  <Navbar :logo="logo_src" :alt="app_name"/>

  <main class="content">
  <router-view/>
  </main>

  <Footer/>

    </div>
</template>


<script>
  import Navbar from './components/Navbar.vue';
  import Footer from './components/Footer.vue'


  export default {
    components: {
      Navbar,
      Footer
    },
    data(){
      return {
        logo_src: "img/logo.png",
        app_name: "Make Your Burguer"
      }
    }
  }
</script>


<style>
  * {
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing:  border-box;
  }

  .main-container {
    margin: 50px;
    min-height: 250px;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }

  #app {
  display: flex;
  flex-direction: column;
  min-height: 100vh; /* força ocupar 100% da altura da tela */
}

.content {
  flex: 1; /* faz o conteúdo crescer e empurra o footer para baixo */
}

</style>
