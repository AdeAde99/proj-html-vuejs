<template>
  <div>
    <div v-for="slide in arrSlides" :key="slide">
      <img :src="slide.img" alt="">
      <h1>{{ slide.title }}</h1>
      <h2> {{ slide.subTitle }} </h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'iacademySlider',
  data () {
    return {
      arrSlides: [
        {
          img: '../assets/img/h5-slide-1-background.jpg',
          title: 'lorem',
          subTitle: ''
        },
        {
          img: '../assets/img/h5-slide-2-background.jpg',
          title: '',
          subTitle: ''
        },
        {
          img: '../assets/img/h5-slide-3-background.jpg',
          title: '',
          subTitle: ''
        }
      ]
    }
  }
}
</script>

<style>
</style>
