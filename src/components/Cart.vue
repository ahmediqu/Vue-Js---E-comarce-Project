<template>
	<div>
	<h3>Carts</h3> <br><hr>
	<ul class="list-group">
		<li class="list-group-item" v-for="(item,index) in items" :key="item"> {{item.title}} - {{item.price}} </li>
	</ul>
</div>
</template>

<script>
	export default {
 
	}
</script>

<style>
	
</style>