<template>
  <DefaultLayout>
    <h1>Posts</h1>
    <LatestPosts/>
  </DefaultLayout>
</template>

<script>
import LatestPosts from '~/components/LatestPosts.vue';
 
export default {
  components: {
    LatestPosts
  }
};
</script>