<template>
    <div>
        Hook
    </div>
</template>

<script>
import {
    onBeforeMount,
    onMounted,
    onBeforeUnmount,
    onUnmounted
} from 'vue'

export default {
    // beforeMount() {
    // },
    // mounted() {
    // },
    // beforeUnmount() {
    // },
    // unmounted() {
    // },
    setup() {
        onBeforeMount(() => {
            console.log('onBeforeMount');
        })

        onMounted(() => {
            console.log('onMounted');
        })

        onBeforeUnmount(() => {
            console.log('onBeforeUnmount');
        })

        onUnmounted(() => {
            console.log('onUnmounted');
        })
    },
}
</script>
