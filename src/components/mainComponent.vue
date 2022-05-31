<template>
  <main>
    <jumbotronTop />

    <logisticSectionComponent />
    
    <theCompanySectionComponent />

    <partnersSectionComponent />

    <latestNewsSectionComponent />

    <newsletterComponent />

    <getInTouchSectionComponent />

  </main>
</template>

<script>
import jumbotronTop from './components_for_main/jumbotronTop.vue'
import logisticSectionComponent from './components_for_main/logisticSectionComponent.vue'
import theCompanySectionComponent from './components_for_main/theCompanySectionComponent.vue'
import partnersSectionComponent from './components_for_main/partnersSectionComponent.vue'
import latestNewsSectionComponent from './components_for_main/latestNewsSectionComponent.vue'
import newsletterComponent from './components_for_main/newsletterComponent.vue'
import getInTouchSectionComponent from './components_for_main/getInTouchSectionComponent.vue'


export default {
  name: 'mainComponent',
  components: {
    jumbotronTop,
    logisticSectionComponent,
    theCompanySectionComponent,
    partnersSectionComponent,
    latestNewsSectionComponent,
    newsletterComponent,
    getInTouchSectionComponent
  }
}
</script>

<style>

</style>