<template>
  <section class="blog-sh">
    <h2>From The Blog</h2>
    <div class="blog-content">
        <div class="blog" v-for="(blogDa, index) in blogData" :key="index">
        <figure>
            <img :src="blogDa.img" alt="">
            <figcaption>{{blogDa.title}}</figcaption>
        </figure>
        <p>
            {{blogDa.content}}
        </p>
    </div>
    </div>
  </section>
</template>

<script setup>
import './blog.css'
import {reactive} from 'vue'
import pl from "../../assets/place.jpg"

const blogData = reactive([
    {title: "Web Design", content: "Sed porttitor lectus nibh. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Curabitur aliquet quam id dui posuere blandit. Cras ultricies ligula sed magna", img: pl},
    {title: "Web Design", content: "Sed porttitor lectus nibh. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Curabitur aliquet quam id dui posuere blandit. Cras ultricies ligula sed magna", img: pl}
])
</script>