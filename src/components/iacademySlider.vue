<template>
  <div class="ciao">
    <div v-for="slide in arrSlides" :key="slide" class="slideContainer">
      <img :src="slide.img" alt="">
      <div class="slideText">
        <h1>{{ slide.title }}</h1>
        <h2> {{ slide.subTitle }} </h2>
      </div>
    </div>
  </div>
</template>

<script>
import slide1Background from '../assets/img/h5-slide-1-background.jpg'
import slide2Background from '../assets/img/h5-slide-2-background.jpg'
import slide3Background from '../assets/img/h5-slide-3-background.jpg'

export default {
  name: 'iacademySlider',
  data () {
    return {
      arrSlides: [
        {
          img: slide3Background,
          title: 'Contemporary Ideas',
          subTitle: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, voluptas reprehenderit dolor veritatis explicabo aliquam, pariatur, dignissimos tenetur possimus sit dolore dolorem officiis vel hic amet eum totam perspiciatis minus.'
        },
        {
          img: slide2Background,
          title: 'Lorem Lorem',
          subTitle: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, voluptas reprehenderit dolor veritatis explicabo aliquam, pariatur, dignissimos tenetur possimus sit dolore dolorem officiis vel hic amet eum totam perspiciatis minus.'
        },
        {
          img: slide1Background,
          title: 'Lorem Lorem',
          subTitle: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero, voluptas reprehenderit dolor veritatis explicabo aliquam, pariatur, dignissimos tenetur possimus sit dolore dolorem officiis vel hic amet eum totam perspiciatis minus.'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.slideText {
  position: absolute;
  top: 0;

  display: flex;
  justify-content: center;
  flex-direction: column;

  color: white;

  h1 {
    font-family: serif;
  }
  h1, h2 {
    text-align: center;
    font-weight: 100;
  }
}
</style>
