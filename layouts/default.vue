<template>
  <div id='app section'>
    <nav-bar />
    <nuxt />
    <div class="container">
  <div class="notification">
    This container is <strong>centered</strong> on desktop.
  </div>
</div>
  </div>
</template>


<script>
  import NavBar from '~/components/NavBar.vue'
  export default {
    components: { 
      NavBar
    }
  }
</script>

<style>

</style>
