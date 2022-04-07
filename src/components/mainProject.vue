<template>
  <main>
      <headerNavbar />
  </main>
</template>

<script>
import headerNavbar from '@/components/headerNavbar.vue'

export default {
  name: 'mainProject',
  components: {
    headerNavbar
  }
}
</script>

<style scoped lang="scss">
  main {
    position: relative;
  }
  headerNavbar {
    position: fixed;
  }
</style>
