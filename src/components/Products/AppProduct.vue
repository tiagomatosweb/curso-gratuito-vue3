<template>
    <div>
        Produto
    </div>
</template>

<script>
import CalculateDiscountMixin from '@/components/Products/CalculateDiscountMixin';

export default {
    mixins: [CalculateDiscountMixin],
    created() {
        this.calculateDiscount()
    },
    methods: {
    }
}
</script>
