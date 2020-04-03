<template>
<nuxt-link :to="'jokes/' + id">
  <div class="border-b border-b-2 border-gray-300 py-4 ">
      <p>{{ joke }}</p>
  </div>
</nuxt-link>
</template>

<script>
export default {
  name: 'Joke',
  props: ['joke', 'id']
}
</script>

<style>

</style>