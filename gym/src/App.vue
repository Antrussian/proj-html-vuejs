<template>
  <div id="app">
    <Header :menuItems="menuItems" />
    <Slogan />
    <Cta />
    <ValueProposition/>
    <RealResults :reviews="reviews" />
    
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Slogan from './components/Slogan.vue';
import Cta from './components/Cta.vue';
import ValueProposition from './components/ValueProposition.vue';
import RealResults from './components/RealResults.vue';

export default {
  components: {
    Header,
    Slogan,
    Cta,
    ValueProposition,
    RealResults,
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

      reviews: [
      {
        id: 1,
        photo: 'blog6-600x600.jpg',
        text: 'A wonderful experience at the gym. I achieved great results!',
        author: 'John Doe',
      },
        {
          id: 2,
          photo: 'blog6-600x600.jpg',
          text: 'The trainers are amazing, and the atmosphere is fantastic.',
          author: 'Jane Smith',
        },

        {
          id: 3,
          photo: 'blog6-600x600.jpg',
          text: 'The trainers are amazing, and the atmosphere is fantastic.',
          author: 'Jane Smith',
        },
        {
          id: 4,
          photo: 'path_to_photo2.jpg',
          text: 'The trainers are amazing, and the atmosphere is fantastic.',
          author: 'Jane Smith',
        },

      ],
    };
  },
};
   
</script>

<style>

</style>
