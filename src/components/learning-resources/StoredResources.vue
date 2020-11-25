<template>
  <ul>
    <learning-resource
      v-for="res in resources"
      :key="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    >
    </learning-resource>
  </ul>
</template>

<script>
import LearningResource from './LearningResources';

export default {
  components: { LearningResource },
  props: ['resources'],

  commponents: {
    LearningResource,
  },
};
</script>

<style scoped>
  ul {
    list-style: none;
    margin: 0 auto;
    padding: 0;
    max-width: 40rem;
  }
</style>