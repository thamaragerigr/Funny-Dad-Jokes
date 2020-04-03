<template>
      <div class="nav ">
        <nuxt-link v-if="main" to="/" class="brand">
        <span>funny</span><br>
        <span>dad</span><br>
        <span>jokes</span></nuxt-link>
        <nav>
          <nuxt-link class="nav-item" to="/">Home</nuxt-link>
          <nuxt-link class="nav-item" to="/jokes">Jokes</nuxt-link>
          <nuxt-link class="nav-item" to="/about">About</nuxt-link>
        </nav>
      </div>
</template>
    

<script>
  export default {
    name: 'NavBar',
    computed:{
      main(){
          return this.$route.path !== '/'
      }
  }
  }
</script>
