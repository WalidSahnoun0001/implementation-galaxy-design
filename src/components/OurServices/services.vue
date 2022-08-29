<template>
  <section class="services">
    <div class="service" v-for="(service, index) in data" :key="index">
        <span><i :class="service.icon"></i></span>
        <h3>{{service.title}}</h3>
        <p>{{service.content}}</p>
    </div>
    <div class="wisdom">
        <p>"I want to make beautiful things, even if nobody cares, as opposed to ugly things. That's my intent."</p>
    </div>
  </section>
</template>

<script setup>
    import './services.css'
    import {reactive} from 'vue'

    const data = reactive([
        {title: "Web Design", content: "Lorem ispum dolor sit amet est oben dis", icon: "fa-brands fa-css3"},
        {title: "Graphic Design", content: "Lorem ispum dolor sit amet est oben dis", icon: "fa-solid fa-pen-nib"},
        {title: "Photography", content: "Lorem ispum dolor sit amet est oben dis", icon: "fa-solid fa-camera"}
    ])
</script>
