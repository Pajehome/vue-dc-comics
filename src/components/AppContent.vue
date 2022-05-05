<template>
  <div class="jumbotron">
   <button>CURRENT SERIES</button>
  </div>
</template>

<script>
export default {
  name: 'AppContent',
}
</script>


<style scoped lang="scss">
@import '../style/variables';

.jumbotron{
  background-image: url(../assets/img/jumbotron.jpg);
  height: 250px;
  background-size: cover;
  position: relative;
    
    button{
      @include current-series;
    }
}


</style>