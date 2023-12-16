<script lang="ts" >
import { useProductsStore } from '@/stores/products';
import { mapState } from 'pinia';
import ProductCard from './ProductCard.vue';

export default {
  components: {
    ProductCard
  },
  computed: {
    ...mapState(useProductsStore, ['products'])
  }
}
</script>

<template>
  

  <v-col 
      :sm="6"
      :xs="12"
      :md="4"
      v-for="product in products" 
      :key="product.id"  >
    <ProductCard  :product="product"  />
    
  </v-col>

</template>