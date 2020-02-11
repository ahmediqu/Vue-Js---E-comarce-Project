<template>
	<div>
	<h3>Products</h3> <br><hr>
          <div class="row">

            <div class="col-md-4" v-for="(item,index) in items" :key="index">
              <div class="card">
                <img class="card-img-top" :src="item.photo" alt="Card image cap">
                <div class="card-body">
                  <h5 class="card-title text-center">{{ item.title}}</h5>
                  <p class="card-text text-center">Some quick example.</p>
                  
                </div>
                <div class="card-footer">
                  <a href="#" class="btn btn-primary">{{ item.price }} {{ index }}</a>
                  <a href="#" class="btn btn-primary float-right">Add</a>
                </div>
              </div>
            </div>

          </div>
          </div>
</template>

<script>
	export default {
 		props: ['items']
	}
</script>

<style>
	
</style>