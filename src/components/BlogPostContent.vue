<template>
    <section>
        <h1>{{$page.blogPost.title}}</h1>
        <p>{{$page.blogPost.date}}</p>
        <ul class="list__no-style">
            <li v-for="tag in $page.blogPost.tags" :key="tag.id">{{tag}}</li>
        </ul>
        <div class="post--item" v-html="$page.blogPost.content" />
    </section>
</template>


<style>

/* this one will work on images in first level - for deeper levels use '.post--img' class */
.post--item > img {
    border-radius: 0.5rem;
    box-shadow: var(--shadow-soft);
}

</style>