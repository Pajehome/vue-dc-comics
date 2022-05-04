<template>
  <div class="content primary-color">	&rarr; Content goes here &larr;</div>
</template>

<script>
export default {
  name: 'AppContent',
}
</script>


<style scoped lang="scss">
@import '../style/variables';

.content{
    @include container;
    background: $aboveNav-color;
    padding: $padding;   
    @include primary-color;
}


</style>