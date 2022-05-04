<template>
  <div id="app">
    <AppHeader/>
    <main>
       <AppContent/>
       <AppGrid/>
    </main>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppGrid from './components/AppGrid.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  name: 'App',
  components: {
    AppHeader,
    AppContent,
    AppGrid,
    AppFooter,
  }
}
</script>

<style lang="scss">
@import './style/general';
</style>
