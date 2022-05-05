<template>
    <div class="prod-card">
        <img :src="immagine" :alt="titolo">
        <h3>{{titolo}}</h3>
    </div>
</template>


<script>
export default {
    name: 'ProductCard',
    props: ['immagine','titolo'],
}
</script>
<style lang="scss" scoped>
@import "../style/variables";
.prod-card {
	flex-basis: 25%;
	padding: 20px;
	background-color: white;
	
	img {
		display: block;
	}
}
</style>