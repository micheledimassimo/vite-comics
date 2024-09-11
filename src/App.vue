<script>

import AppHeader from './components/AppHeader.vue';

import AppFirstSection from './components/AppFirstSection.vue';
import AppSecondSection from './components/AppSecondSection.vue';
import AppFooter from './components/AppFooter.vue';
import AppJumbotron from './components/AppJumbotron.vue';






export default {
  data() {
    return { 
      
    }
  },
  components: {
    AppHeader,
    AppJumbotron,
    AppFirstSection,
    AppSecondSection,
    AppFooter
  },
    methods: {
    
  }
}
</script>

<template>
  
  <AppHeader />
  
  <AppJumbotron />
  
  <AppFirstSection />

  <AppSecondSection />

  <AppFooter />
</template>

<style scoped>

</style>
