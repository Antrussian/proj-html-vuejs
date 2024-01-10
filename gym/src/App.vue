<template>
  <div id="app">
    <Header :menuItems="menuItems" />
    <Slogan />
    <Cta />
    <ValueProposition/>
    
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Slogan from './components/Slogan.vue';
import Cta from './components/Cta.vue';
import ValueProposition from './components/ValueProposition.vue';

export default {
  components: {
    Header,
    Slogan,
    Cta,
    ValueProposition,
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

</style>
