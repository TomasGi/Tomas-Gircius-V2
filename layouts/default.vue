<template>
  <div>
    <Header/>
    <Nav/>
    <!-- <div class="container"> -->
      <nuxt/>
    <!-- </div> -->
  </div>
</template>

<script>
import Header from './partials/header'
import Nav from './partials/navigation'
  export default {
    components: {
      Header,
      Nav
    }
  }
</script>

<style lang="scss" scoped>

</style>