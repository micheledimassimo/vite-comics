<script>

import AppHeader from './components/AppHeader.vue';
import AppFirstSection from './components/AppFirstSection.vue';
import AppSecondSection from './components/AppSecondSection.vue';
import AppFooter from './components/AppFooter.vue';



export default {
  data() {
    return { 
      
    }
  },
  components: {
    AppHeader,
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
    
  <AppFirstSection />

  <AppSecondSection />

  <AppFooter />
</template>

<style scoped>

</style>
