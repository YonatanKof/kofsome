<template>
    <DefaultLayout :bgImage="$page.blogPost.image">
        <div id="kof" v-if="$page.blogPost.flip" dir="rtl">
          <!-- BlogPostContent is in other component for direction while header is unchanged  -->
          <BlogPostContent/>
        </div>
        <div id="kof" v-else dir="ltr">        
          <BlogPostContent/>
        </div>
    </DefaultLayout>
</template>

<script>
import BlogPostContent from '~/components/BlogPostContent.vue';

export default {
  components: {
    BlogPostContent
  }
};

</script>
<page-query>
 query Post ($path: String!) {	
  blogPost (path: $path){
    title
    date (format:"MMM DD, YYYY")
    tags
    content
    image
    flip
  }
}
</page-query>