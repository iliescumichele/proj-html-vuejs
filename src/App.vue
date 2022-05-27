<template>
  <div id="app">
    <headerComponent />

    <mainComponent />

    <footerComponent />

  </div>
</template>

<script>
import headerComponent from './components/headerComponent.vue'
import mainComponent from './components/mainComponent.vue'
import footerComponent from './components/footerComponent.vue'


export default {
  name: 'App',
  components: {
    headerComponent,
    mainComponent,
    footerComponent
  }
}
</script>

<style lang="scss">
#app {
  @import './assets/style/general.scss';
  @import './assets/style/vars.scss';
  
}
</style>
