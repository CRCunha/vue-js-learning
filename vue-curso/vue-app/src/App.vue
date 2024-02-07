<template>
  <HeaderComponent />
  <PauseComponent v-show="showPause" />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import PauseComponent from './components/PauseComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    PauseComponent,
  },

  data() {
    return {
      showPause: true,
    };
  },
};
</script>

<style>
#app {
  font-family: 'Montserrat', sans-serif;
  width: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
}
</style>
