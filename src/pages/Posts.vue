<template>
  <layout>
    <h1>Posts</h1>
    <LatestPosts/>
  </layout>
</template>

<script>
import LatestPosts from '../components/LatestPosts.vue';
 
export default {
  components: {
    LatestPosts
  }
};
</script>