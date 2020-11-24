<template>
  <ul>
    <LearningResouce
      v-for="res in storedResoucers"
      :key="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    >
    {{child}}
    </LearningResouce>
  </ul>
</template>

<script>
import LearningResouce from './components/learning-resources/LearningResource.vue';

export default {
  components: {
    LearningResouce,
  },

  data() {
    return {
      storedResoucers: [
        {
          id: 'official-guid',
          title: 'Official Guid',
          description: 'The official VUe js documentation',
          link: 'https://vuejs.org',
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn how to google...',
          link: 'https://google.com',
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>