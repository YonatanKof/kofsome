<template>
  <div class="layout">
    <header class="header">
      <strong>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
    </header>
    <slot/>
  </div>
</template>

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
    justify-content: space-around;
}
</style>
