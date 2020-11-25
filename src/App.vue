<template>
  <application-header/>
  <stored-resources :resources="storedResoucers"/>
</template>

<script>
import StoredResources from './components/learning-resources/StoredResources';
import ApplicationHeader from './components/hearder/ApplicationHeader';

export default {
  components: {
    StoredResources,
    ApplicationHeader
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

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');

  * {
    box-sizing: border-box;
  }

  html {
    font-family: 'Roboto', sans-serif;
  }

  body {
    margin: 0;
  }
</style>