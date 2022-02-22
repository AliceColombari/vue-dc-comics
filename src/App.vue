<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>
    <SectionCurrentSeries/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';
import SectionCurrentSeries from './components/SectionCurrentSeries.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
    SectionCurrentSeries
  }
}
</script>

<style lang="scss">
  @import "./assets/style/general.scss"; 
</style>
