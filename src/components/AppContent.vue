<template>
  <div class="content">	&rarr; Content goes here &larr;</div>
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
    color: $primary-text
}

</style>