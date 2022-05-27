<template>
  <div id="app">

    <HeaderComponent/>

    <JumbotronComponent/>

    <MainComponent/>

    <FooterComponent/>

  </div>
</template>


<script>
import HeaderComponent from './components/HeaderComponent.vue';
import JumbotronComponent from './components/JumbotronComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';


export default {
  name: 'App',
  components: {
    HeaderComponent,
    JumbotronComponent,
    MainComponent,
    FooterComponent
}
}
</script>


<style lang="scss">

  @import './assets/style/vars';
  @import './assets/style/general';
  @import './assets/style/mixins';

  ul {
    list-style: none;
    
    a {
    text-decoration: none;
    color: #000000
    }
  }

  

</style>
