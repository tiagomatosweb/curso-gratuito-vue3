<template>
    <div>
        <BaseAlert
            :variant="variant"
        >
            {{ text }}
        </BaseAlert>
    </div>
</template>

<script>
import BaseAlert from '@/components/BaseAlert';
export default {
    name: 'App',
    components: { BaseAlert },
    data() {
        return {
            variant: 'success',
            text: 'Seu formulário foi enviado'
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
