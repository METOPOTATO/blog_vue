<template>
 <p>{{ product.name }}</p>
</template>

<script>
export default {
  name: 'product',
  props:{
    product:{
      type: Object,
    }
  },
  data(){
    return {
      text: 'Product'
    }
  }
}
</script>

<style>

</style>