<template>
  <nav>
    <div>
        <img src="" alt="Logo">
    </div>
    <div>
        <a href="">Inicio</a>
        <a href="">Sobre</a>
        <a href="">Projetos</a>
        <a href="">Contato</a>
    </div> 
  </nav>
  <router-view/>

  <footer>

  </footer>
</template>

<script>

</script>

<style>
*{
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100%;
  background-color: white;
}

nav {
  display:sticky;
  top: 0;
  height: 80px;
  width: 100%;
  box-shadow: 0px 10px 10px -15px #111; 
  background-color: white;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
