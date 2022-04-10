<template>
<!--Qui verranno inseriti la navbar, il main e il footer.-->
  <div id="app">
    <mainProject />
    <iacademySlider />
    <iacademyFooter />
  </div>
</template>

<script>

import mainProject from '@/components/mainProject.vue'
import iacademySlider from '@/components/iacademySlider.vue'
import iacademyFooter from '@/components/iacademyFooter.vue'

export default {
  name: 'App',
  components: {
    mainProject,
    iacademySlider,
    iacademyFooter
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;500;600;700;800&display=swap');

#app {
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Open Sans', sans-serif;
  }
}
</style>
