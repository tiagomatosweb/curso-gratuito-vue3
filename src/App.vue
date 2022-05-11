<template>
    <div>
        <TheHeader>
            <template v-slot:description>
                <p>dasds</p>
            </template>

            Content do header - menu ...
        </TheHeader>
    </div>
</template>

<script>
import TheHeader from '@/components/TheHeader';
export default {
    name: 'App',
    components: { TheHeader },
    data() {
        return {
        }
    },
    beforeUpdate() {},
    updated() {},
    beforeCreate() {},
    created() {},
    beforeMount() {},
    mounted() {},
    watch: {},
    computed: {},
    methods: {}
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin: 60px;
}
</style>
