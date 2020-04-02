<template>
<div>
  <div class="red-line"></div>

  <div id='app'>
    <nav-bar />
    <nuxt />
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
