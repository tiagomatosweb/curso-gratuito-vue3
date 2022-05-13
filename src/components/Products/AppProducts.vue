<template>
    <div>
        <AppProduct
            v-for="product in $store.state.products"
            :key="product.id"
            :product="product"
        />
    </div>
</template>
<script>
import AppProduct from '@/components/Products/AppProduct';
export default {
    components: { AppProduct }
}
</script>
