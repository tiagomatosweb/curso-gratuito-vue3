<template>
  <img alt="Vue logo" src="./assets/logo.png">
    <button @click="updateUser()">
        Atualizar perfil
    </button>
  <HelloWorld
      user=""
      msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
    data() {
      return {
      }
    },

    methods: {
        updateUser() {
            const newUser = {
                first_name: 'Tiago',
                last_name: 'Matos',
                email: 'tiago@tiago.com'
            }
            this.$store.commit('storeUser', newUser)
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
  margin-top: 60px;
}
</style>
