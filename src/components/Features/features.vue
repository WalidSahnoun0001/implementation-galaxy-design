<template>
  <section class="features">
    <div class="feature" v-for="(feature, index) in features" :key="index">
        <figure>
            <img :src="feature.img" alt="">
            <figcaption>{{feature.title}}</figcaption>
        </figure>
        <p>{{feature.content}}</p>
    </div>
  </section>
</template>

<script setup>
    import './features.css'
    import {reactive} from 'vue'
    import pl from '../../assets/place.jpg'

    const features = reactive([
        {title: "Cool Image", content: "Galaxy Corp.", img: pl},
        {title: "Great Picture", content: "Galaxy Corp.", img: pl},
        {title: "Cool Image", content: "Galaxy Corp.", img: pl},
    ])

</script>

<style>

</style>