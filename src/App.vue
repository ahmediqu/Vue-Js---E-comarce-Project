<template>
  <div id="app">
    <div class="container shadow">
      <Navbar></Navbar>
    </div>
    <div class="container mt-5">
      <div class="row">
        <div class="col-md-9">
          <Product :items="items"></Product>
        </div>
        <div class="col-md-3">
          <Cart :items="cart"></Cart>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar'
import Cart from './components/Cart'
import Product from './components/Product'
import data from './data.js'
export default {
 components: {
  Navbar,
  Cart,
  Product
 },
 data() {
  return{
    items: [],
    cart: [{
      id: 1,
      title: 'test',
      print: 20.3,
      photo: 'http://dummyimage.com/209x169.bmp/ff4444/ffffff'
    }]
  }
 },
 mounted() {
  this.items = data
 }

}
</script>

<style>

</style>
