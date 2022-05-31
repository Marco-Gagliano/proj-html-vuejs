<template>
  
  <main>
    <ResultComponent/>
    <ServiceComponent/>
    <TeamComponent/>
    <NewsComponent/>
    <NewsletterComponent/>
    <MessaggeComponent/>
  </main>

</template>


<script>

import ResultComponent from './ResultComponent.vue'
import ServiceComponent from './ServiceComponent.vue'
import TeamComponent from './TeamComponent.vue'
import NewsComponent from './NewsComponent.vue'
import NewsletterComponent from './NewsletterComponent.vue'
import MessaggeComponent from './MessaggeComponent.vue'


export default {
    name: "MainComponent",
    components: { ResultComponent, 
                  ServiceComponent, 
                  TeamComponent, 
                  NewsComponent, 
                  NewsletterComponent, 
                  MessaggeComponent}
}
</script>

<style lang="scss" scoped>


</style>