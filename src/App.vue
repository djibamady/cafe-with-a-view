<template>
  <div id="app">
    <app-hello
      :msg="messageFromApp"
      :contenu="contentFromApp"
      :costOfApples="appleCostFromApp"
      :costOfBananas="bananaCostFromApp"
      :costOfCoconuts="coconutCostFromApp"
    ></app-hello>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    // eslint-disable-next-line vue/no-unused-components
    'app-hello': HelloWorld
  },
  data() {
    return {
      messageFromApp: 'Bonjour depuis App.vue',
      contentFromApp: 'Contenu personnalisé depuis App.vue',
      appleCostFromApp: 6,
      bananaCostFromApp: 2,
      coconutCostFromApp: 8
    };
  }
};
</script>

<style>
#app {
  text-align: center;
  padding: 20px;
}
</style>
