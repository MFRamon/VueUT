<template>
  <div>
    <ul>
      <li :class="{ active: star <= initialGrade}"
      :key="star" v-for="star in maxStars" class="star"></li>
    </ul>
    <div class="summary">{{ initialGrade }} of {{ maxStars }}</div>
  </div>
</template>

<script>
export default {
  props: {
    maxStars: {
      type: Number,
    },
    initialGrade: {
      type: Number,
    },
  },
};
</script>

<style>

</style>
