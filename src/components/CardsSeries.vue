<template>
    <div class="prod-card">
        <img :src="immagine" :alt="titolo">
        <h3>{{titolo}}</h3>
    </div>
</template>


<script>
export default {
    name: 'CardsSeries',
    props: ['immagine','titolo'],
}
</script>
<style lang="scss" scoped>
@import "../style/variables";
.prod-card {
	flex-basis: 25%;
	padding: 20px;
    @include primary-color;
	img {
		display: block;
        width: 200px;
        height: 205px;
        object-fit: cover;
        object-position: top;
	}
}
</style>