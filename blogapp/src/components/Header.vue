<template>
  <header><h1>{{ titleHeader }}</h1></header>
</template>

<script>
export default {
  name: 'comp-header',
  data(){
    return {
      text: 'Header'
    }
  },
  props:{
    titleHeader: String
  }
}
</script>

<style>

</style>