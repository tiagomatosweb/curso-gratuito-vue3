<template>
  <nav>
    <RouterLink to="/">Home</RouterLink> |
    <RouterLink :to="rotaDinamica">Serviços</RouterLink> |
    <RouterLink to="/usuarios/10">Usuario</RouterLink> |
    <router-link to="/about">About</router-link>
  </nav>

  <RouterView/>
</template>

<script>
export default {
    data() {
        return {
            rotaDinamica: { name: 'servicos' }
        }
    },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
