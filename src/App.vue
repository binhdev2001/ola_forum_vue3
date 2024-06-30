<template>
  <router-view />
</template>
<script>
import HeaderApp from './components/HeaderApp.vue';
import FooterApp from './components/FooterApp.vue';
export default {
  name: 'App',
  components: {
    HeaderApp,
    FooterApp
  }
};
</script>

