<template>
<!--Qui verranno inseriti la navbar, il main e il footer.-->
  <div id="app">
    <mainProject />
    <iacademySlider />
  </div>
</template>

<script>

import mainProject from '@/components/mainProject.vue'
import iacademySlider from '@/components/iacademySlider.vue'

export default {
  name: 'App',
  components: {
    mainProject,
    iacademySlider
  }
}
</script>

<style lang="scss">
#app {
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  position: relative;
}
</style>
