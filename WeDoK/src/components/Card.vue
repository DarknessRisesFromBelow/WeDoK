<script setup>
	import {ref} from 'vue'

	const cardContent = ref("populate this board");
	const importance = ref(0);
	const label = ref("work");
</script>

<template>
	<div class="cardContainer">
		<h2 style="text-align: center; padding-top: 1vh">{{cardContent}}</h2>
	</div>
</template>

<style scoped>
	.cardContainer{
		background: rgb(60,60,60);
		box-shadow: 0 0 4px 0.1px black;
		border-radius: 0.7em;
		height: 8lvh
	}
</style>