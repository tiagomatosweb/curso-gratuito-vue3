<template>
    <AppHook v-if="showAppHook" />

    <button @click="showAppHook = !showAppHook">
        Toggle
    </button>

    <h5>User</h5>
    {{ user.first_name }}
    {{ user.last_name }}
    <br><br>
    <h6>Full name</h6>
    {{ fullName }}

    <button @click="user.first_name = 'Sansa'">Atualizar</button>
</template>

<script>
import { ref, computed, watch } from 'vue';
import AppHook from '@/components/AppHook';

export default {
    name: 'App',
    components: { AppHook },
    setup() {
        const user = ref({
            first_name: 'Jon',
            last_name: 'Snow'
        })

        const showAppHook = ref(true)

        const fullName = computed(() => `${user.value.first_name} ${user.value.last_name}`)

        watch(() => user.value.first_name, () => {
            console.log('Logica cabulosa');
        })

        return {
            user,
            fullName,
            showAppHook,
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
