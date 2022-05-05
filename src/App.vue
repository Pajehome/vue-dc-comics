<template>
  <div id="app">
    <AppHeader/>
    <main>
       <AppContent/>
       <AppCards/>
       <AppGrid/>
    </main>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppCards from './components/AppCards.vue'
import AppGrid from './components/AppGrid.vue'
import AppFooter from './components/AppFooter.vue'



export default {
  name: 'App',
  components: {
    AppHeader,
    AppContent,
    AppCards,
    AppGrid,
    AppFooter,
  }
}
</script>

<style lang="scss">
@import './style/general';
</style>
