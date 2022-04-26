<template>
<div>
  <header>
    <span>My Site</span>
    <span>Link?</span>
  </header>
  <main>
    <Nuxt />
  </main>
  <footer>
    Footer &copy;2022
  </footer>
</div>
</template>

<script>
export default {
  name: "default.vue",
}
</script>

<style>

  html,body{
    font-family: "Comic Sans MS", cursive;
  }

  header{
    display:flex;
    flex-flow: row nowrap;
    justify-content: space-between;
  }

  main{
    min-height: 100vh;
  }

  footer{
    display:flex;
    justify-content: center;
    align-items: center;
  }
</style>
