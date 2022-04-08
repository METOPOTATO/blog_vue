<template>
  <Header v-bind:titleHeader="title"/>
  <img alt="Vue logo" src="./assets/logo.png">
  <ListProduct v-bind:listProduct="listProduct"/>
  <Footer/>
</template>

<script>
import ListProduct from './components/ListProducts.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    ListProduct
  },
  data (){
    return {
      title: "Hello This is header",
      listProduct:[
        {id:1, name: 'book', active:true},
        {id:2, name: 'table', active:true},
        {id:3, name: 'pen', active:true},
        {id:4, name: 'mouse', active:false},
        {id:5, name: 'phone', active:true},
        {id:6, name: 'bottle', active:false},
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
