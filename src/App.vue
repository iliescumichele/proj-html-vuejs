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
  @import './assets/style/general.scss';
  @import './assets/style/vars.scss';
  @import '~bootstrap/scss/bootstrap.scss';
  @import '~@fortawesome/fontawesome-free/css/all.min.css';

</style>
