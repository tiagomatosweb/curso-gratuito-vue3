<template>
    <AppProduct />
    {{ name }}
  <img @click="changeName()" alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import AppProduct from '@/components/Products/AppProduct';

export default {
  name: 'App',
  components: {
      AppProduct,
    HelloWorld
  },
  setup() {
      // lgoica cabulosa
      let name = 'Tiago'

      const changeName = () => {
          //logica cabulosa
          alert('chegou')
          name = 'Jon Snow'
      }

      return {
          name,
          changeName
      }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
