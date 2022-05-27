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
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
import JumbotronComponent from './components/JumbotronComponent.vue';


export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
    JumbotronComponent
}
}
</script>


<style lang="scss">

  @import './assets/style/vars';
  @import './assets/style/general';
  @import './assets/style/mixins';

</style>
