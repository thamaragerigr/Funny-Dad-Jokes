<template>
  <div class="mt-12 ml-4">
      <nuxt-link to="/jokes" class="flex-shrink-0 bg-red opacity-75 hover:opacity-100 border-none text-sm border-4 text-white py-1 px-2 rounded">Back to jokes</nuxt-link>
      <div class="m-10">
      <h2 class=" p-6 bg-gray-100 rounded">{{ joke }}</h2>
      <small>Joke ID: {{ $route.params.id }}</small>
      </div>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  data() {
      return {
          joke: {}
      }
  },
  async created(){
       const config = {
           headers: {
               Accept: 'application/json'
           }
       };
       try {
        const res = await axios.get(`https://icanhazdadjoke.com/j/${this.$route.params.id}`, config);
        this.joke = res.data.joke;
       } catch (err) {
         console.log(err);
       }

    },
     head(){
        return {
            title: this.joke,
            meta: [ {
                hid:'description',
                name: 'description',
                content: 'Best dad jokes'
               }
            ]
        }
    }
}
</script>

<style>

</style>