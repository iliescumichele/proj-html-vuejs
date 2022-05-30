<template>
  <main>
    <jumbotronTop />

    <logisticSectionComponent />
    
    <theCompanySectionComponent />

    <partnersSectionComponent />

  </main>
</template>

<script>
import jumbotronTop from './components_for_main/jumbotronTop.vue'
import logisticSectionComponent from './components_for_main/logisticSectionComponent.vue'
import theCompanySectionComponent from './components_for_main/theCompanySectionComponent.vue'
import partnersSectionComponent from './components_for_main/partnersSectionComponent.vue'


export default {
  name: 'mainComponent',
  components: {
    jumbotronTop,
    logisticSectionComponent,
    theCompanySectionComponent,
    partnersSectionComponent
  }
}
</script>

<style>

</style>