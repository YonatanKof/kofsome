<template>
    <DefaultLayout :bgImage="$page.blogPost.image">
        <h1> {{$page.blogPost.title}} </h1>
        <p> {{$page.blogPost.date}} </p>
        <ul class="list__no-style"> 
            <li v-for="tag in $page.blogPost.tags" :key="tag"> {{tag}} </li>
        </ul>   
        <div v-html=" $page.blogPost.content"/>
    </DefaultLayout>
</template>

<page-query>
 query Post ($path: String!) {	
  blogPost (path: $path){
    title
    date (format:"MMM DD, YYYY")
    tags
    content
    image
  }
}
</page-query>