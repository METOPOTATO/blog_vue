<template>
  <div class="list-products">
    <Product
        v-for="product in listProduct"
        v-bind:key="product.id"
        v-bind:product="product"
    />
  </div>
</template>


<script>
import Product from './Product.vue';
export default {
  name: 'list-product',
  data(){
      return {

      }
  },
  components:{
    Product
  },
  props:{
      listProduct: {
          type: Array
      }
  }
  
}
</script>

<style>

</style>