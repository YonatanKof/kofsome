<template>
  <div>
    <header class="header">
      <strong>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about/">About</g-link>
        <g-link class="nav__link" to="/posts/">Posts</g-link>
      </nav>
    </header>
    <g-image v-if="bgImage" :src="bgImage"/>
    <div class="layout">
      <slot/>
    </div>
  </div>
</template>

<script> 
export default {
  props: ["bgImage"]
};
</script>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style scoped>
.header{
    align-items: center;
    margin-bottom: 20px;
    height: 80px;
    display: flex;
    justify-content: space-between;
}
</style>