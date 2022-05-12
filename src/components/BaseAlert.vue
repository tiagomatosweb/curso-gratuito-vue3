<template>
    <div :class="baseClass">
        <slot />
    </div>
</template>

<script>
export default {
    props: {
        variant: {
            type: String,
            default: ''
        },
    },

    computed: {
        baseClass() {
            return [
                'alert',
                this.variant ? `alert-${this.variant}` : ''
            ]
        },
    },

    methods: {
    }
}
</script>

<style scoped>
.alert {
    display: flex;
    justify-content: space-between;
    padding: 5px;
    border-radius: 6px;
    color: gray;
    background: #ddd;
}
.alert-success {
    background: #42b983;
    color: #fff;
}
.alert-danger {
    background: red;
    color: #fff;
}
</style>
