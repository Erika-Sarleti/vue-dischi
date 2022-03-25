<template>
  <div id="app">
    <HeaderDisc/>
    <MainDisc/> 
  </div>
</template>

<script>
import HeaderDisc from './components/HeaderDisc.vue';
import MainDisc from './components/MainDisc.vue'

export default {
  name: 'App',
  components: {
    HeaderDisc,
    MainDisc,
  }
}
</script>

<style lang="scss">
@import './assets/styles/variables.scss';
@import './assets/styles/general.scss';
@import 'bootstrap';

</style>
