<template>
  <main>
    <jumbotronTop />

    <logisticSectionComponent />


  </main>
</template>

<script>
import jumbotronTop from './components_for_main/jumbotronTop.vue'
import logisticSectionComponent from './components_for_main/logisticSectionComponent.vue'


export default {
  name: 'mainComponent',
  components: {
    jumbotronTop,
    logisticSectionComponent
  }
}
</script>

<style>

</style>