<template>
  <section>
    <div>
      <h2>Latest posts</h2>
      <article v-for="edge in $static.allBlogPost.edges" :key="edge.node.id">
          <!-- <div v-html=" edge.node.content"/> -->
          <h2> {{edge.node.title}} </h2>
          <p> {{edge.node.date}} </p>
          <ul> 
            <li v-for="tag in edge.node.tags"> {{tag}} </li>
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
ul{
  list-style: none;
  padding: 0;
}
li{
  display: inline;
}

</style>