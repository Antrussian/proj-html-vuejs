<template>
  <div class="real-results-container">
    <div class="row">
      <div v-for="review in reviews" :key="review.id" class="review-card">
        <div class="img-container">
          <img :src="`../../assets/images/${review.photo}`" :alt="`Photo of ${review.author}`" class="img-review" />
        </div>
        <div class="text-container">
          <p class="italic-text">{{ review.text }}</p>
          <p class="author">{{ review.author }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    reviews: Array,
  },
};
</script>

<style>
.real-results-container {
  width: 100%;
  margin: 20px;
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

.img-review {
  width:50px;
}

.row {
  display: flex;
  flex-wrap: wrap;
  width: 80%;
  
}

.review-card {
  width: 48%;
  margin-bottom: 20px;
  display: flex;
}

.img-container {
  width: 50%;
}



.text-container {
  width: 50%;
  padding: 0 10px;
}

.italic-text {
  font-style: italic;
}

.author {
  margin-top: 10px;
  font-weight: bold;
}
</style>
