<template>
  <header>
      <img src="../assets/img/logo-light.png" alt="">
      <ul>
          <li v-for="link in arrLinkNavbar" :key="link">
              <a href="">{{ link.text }}</a>
          </li>
      </ul>
      <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
      <font-awesome-icon icon="fa-solid fa-bag-shopping" />
      <font-awesome-icon icon="fa-solid fa-bars" />
  </header>
</template>

<script>

export default {
  name: 'headerNavbar',
  data () {
    return {
      arrLinkNavbar: [
        {
          text: 'HOME',
          link: ''
        },
        {
          text: 'COURSES',
          link: ''
        },
        {
          text: 'INSTRUCTORS',
          link: ''
        },
        {
          text: 'EVENTS',
          link: ''
        },
        {
          text: 'PAGES',
          link: ''
        },
        {
          text: 'ELEMENTS',
          link: ''
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
template {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
header {
    display: flex;
    align-items: center;
    background-color: aquamarine;
}
ul {
    display: flex;
    list-style: none;
}
a {
    text-decoration: none;
    color: white;
}
.fa-solid {
    color: white;
}
</style>
