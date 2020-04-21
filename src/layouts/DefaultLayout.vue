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
      <transition name="image-fade" appear>
        <main>
          <g-image class="main-cover" v-if="bgImage" :src="bgImage"/>
        </main>
      </transition>
    <div class="layout">
      <transition name="fade" appear>
        <main>
          <slot/> 
        </main>
      </transition>
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

<style>
.image-fade-enter-active {
  transition: all 1s ease;
}

.image-fade-enter {
  transform: scale(1.02);
  opacity: 0;
}
.fade-enter-active {
  transition: opacity .5s;
}

.fade-enter {
  opacity: 0;
}

.header{
  align-items: center;
  display: flex;
  justify-content: space-between;
  max-width: 760px;
  margin: 20px auto;
}
.main-cover{
  height: 400px;
  object-fit: cover;
}
</style>