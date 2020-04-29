<template>
    <section>
        <div>
            <h2>Latest posts</h2>
            <!-- The :dir below is another way to flip text dircertion -->
            <article
                v-for="edge in $static.allBlogPost.edges"
                :key="edge.node.id"
                :dir="`${edge.node.dirction}`"
            >
              <g-link class="main-click" :to="`/posts/${edge.node.slug}`">
                  <g-image :src="`~${edge.node.image.src}`"/>
                  <div class="title">
                    <h3>{{edge.node.title}}</h3>
                    <p><strong>{{edge.node.excerpt}}</strong></p>
                    <p>{{edge.node.date}}</p>
                    <ul class="list__no-style">
                        <li v-for="tag in edge.node.tags" :key="tag.id">{{tag}}</li>
                    </ul>
                  </div>
                </g-link>
            </article>
        </div>
    </section>
</template>


<static-query>
  query LatestPosts {
    allBlogPost (perPage: 5){
        edges{
          node{
            id
            excerpt
            image (width: 760, height: 320, quality: 90)
            title
            date (format:"MMM DD, YYYY")
            tags
            slug
            flip
            dirction
          }
        }
      }
    } 
</static-query>

<style>
article {
    margin-bottom: 32px;
    background-color: var(--bg-card);
    border-radius: 4px;
    overflow: hidden;
    transition: box-shadow .35s;
    box-shadow: var(--shadow);
}
article:hover{
    box-shadow: var(--shadow-hover);
    
}
.main-click{
  color: #1a1a1a;
  display: inline-block;
  text-decoration: none;
}
.title {
  padding: 8px 24px 24px;
}
</style>