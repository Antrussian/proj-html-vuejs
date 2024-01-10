<template>
  <div id="app">
    <Header :menuItems="menuItems" />
 
    <!-- Aggiungi altri componenti se necessario -->
  </div>
</template>

<script>
import Header from './components/Header.vue';


export default {
  components: {
    Header,

  },
  data() {
    return {
      menuItems: [
        { id: 1, label: 'HOME' },
        { id: 2, label: 'ABOUT US' },
        { id: 3, label: 'FACILITIES' },
        { id: 4, label: 'MEMBERSHIP' },
        { id: 5, label: 'TESTIMONIALS' },
        { id: 6, label: 'BLOG' },
      ],
    };
  },
};
</script>

<style>
/* Aggiungi stili globali qui se necessario */
</style>
