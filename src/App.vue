<template>
    <TheHeader v-if="showHeader" />

    <div v-show="showName">
        Nome: {{ firstName }} <br>
        Sobrenome: {{ lastName }}
    </div>

    <div v-if="accessLevel === 'admin'">Usuário Admin</div>
    <div v-else-if="accessLevel === 'marketing'">Usuário Marketing</div>
    <div v-else>Usuário normal</div>

    <img
        alt="Vue logo"
        src="./assets/logo.png"
    >
    <HelloWorld msg="Welcome to Your Vue.js App" />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TheHeader from './components/TheHeader';

export default {
    name: 'App',
    components: {
        HelloWorld,
        TheHeader
    },
    data() {
        return {
            showHeader: true,
            firstName: 'Jon',
            lastName: 'Snow',
            showName: false,
            accessLevel: 'admin'
        }
    }
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
