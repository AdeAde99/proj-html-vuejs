<template>
  <header>
      <img src="../assets/img/logo-light.png" alt="">
      <ul>
          <li v-for="link in arrLinkNavbar" :key="link">
              <a href="">{{ link.text }}</a>
          </li>
      </ul>
      <div>
        <font-awesome-icon icon="fa-solid fa-magnifying-glass" class="whiteIcon iconNav" />
        <font-awesome-icon icon="fa-solid fa-bag-shopping" class="whiteIcon iconNav" />
        <font-awesome-icon icon="fa-solid fa-bars" class="whiteIcon iconNav"/>
      </div>
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
img {
  width: 15%;
}
template {
    margin: 0;
    padding-top: 0;
    box-sizing: border-box;
}
header {
    padding-top: 2rem;

    display: flex;
    align-items: center;
    justify-content: space-around;

    width: 100%;

    position: fixed;
    div {
      display: flex;
      gap: 2rem;

    }
  }
ul {
    display: flex;
    list-style: none;
    gap: 2rem;
}
a {
    text-decoration: none;
    color: white;
    font-size: 1.25em;
    font-weight: 100;
}
.whiteIcon {
    color: white;
    font-size: 1.5em;
    font-weight: 100;
}

</style>
