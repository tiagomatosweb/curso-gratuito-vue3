<template>
    {{ name }} <br><br>

    <h5>User</h5>
    {{ user.first_name }}
    {{ user.last_name }}
    <br><br>
    <h5>Admin</h5>
    {{ admin.first_name }}
    {{ admin.last_name }}
    <br><br>
    <img
        @click="changeName()"
        alt="Vue logo"
        src="./assets/logo.png"
    >
    <HelloWorld msg="Welcome to Your Vue.js App" />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import { ref, reactive } from 'vue';

export default {
    name: 'App',
    components: {
        HelloWorld
    },
    setup() {
        const user = reactive({
            first_name: 'Jon',
            last_name: 'Snow'
        })

        const admin = ref({
            first_name: 'Admin',
            last_name: 'Master'
        })

        const count = ref(0)
        console.log(count);


        // lgoica cabulosa
        let name = 'Tiago'

        const changeName = () => {
            //logica cabulosa
            alert('chegou')
            name = 'Jon Snow'
            user.first_name = 'Sansa'
            admin.value.first_name = 'XXXX'
        }

        return {
            user,
            admin,
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
    color: #2c3e50;
    margin-top: 60px;
}
</style>
