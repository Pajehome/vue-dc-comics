<template>
  <div id="app">
    <AppHeader/>
    <main>
       <AppGrid/>
    </main>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppGrid from './components/AppHeader.vue'
import AppFooter from './components/AppHeader.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppGrid,
    AppFooter,
  }
}
</script>

<style lang="scss">

</style>
