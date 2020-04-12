<template>
  <section>
    <div>
      <h2>Latest posts</h2>
      <article v-for="edge in $static.allBlogPost.edges" :key="edge.node.id">
          <h2> {{edge.node.title}} </h2>
          <p> {{edge.node.date}} </p>
          <ul class="list__no-style"> 
            <li v-for="tag in edge.node.tags" :key="tag"> {{tag}} </li>
          </ul>
          <g-link :to="`/posts/${edge.node.slug}`" >Read more</g-link>
      </article>
    </div>
  </section>
</template>

<static-query>
  query LatestPosts {
    allBlogPost{
        edges{
          node{
            id
            title
            date (format:"MMM DD, YYYY")
            tags
            slug
          }
        }
      }
    } 
</static-query>

<style>
  article{
    margin: 40px 0;
  }
</style>