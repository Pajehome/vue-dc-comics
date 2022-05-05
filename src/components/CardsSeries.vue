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
	flex-basis: 16%;
	padding: 20px 0px;
    @include primary-color;
	img {
		display: block;
        width: 140px;
        height: 140px;
        object-fit: cover;
        object-position: top;
	}
    h3{
    padding-top: 10px;
    font-weight: 400;
    text-transform: uppercase;
    font-size: $font-primary;
    }
}
</style>