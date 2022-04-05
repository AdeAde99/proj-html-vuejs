<template>
<!--Qui verranno inseriti la navbar, il main e il footer.-->
  <div id="app">
    <headerNavbar />
  </div>
</template>

<script>

import headerNavbar from '@/components/headerNavbar.vue'

export default {
  name: 'App',
  components: {
    headerNavbar
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
}
</style>
