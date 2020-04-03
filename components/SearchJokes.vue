<template>
  <form class="w-full max-w-sm" @submit.prevent="onSubmit">
  <div class="flex items-center py-2">
    <input  type="text" v-model="text" placeholder="Search Jokes..." class="appearance-none bg-gray-200 border-none w-full mr-3 py-1 px-2 leading-tight focus:bg-gray-100 rounded">
    <input class="flex-shrink-0 bg-red opacity-75 hover:opacity-100 border-none text-sm border-4 text-white py-1 px-2 rounded" type="submit" value="Search">
  </div>
</form>
</template>

<script>
export default {
  name: "SearchJokes",
  data() {
    return {
      text: ""
    };
  },
  methods: {
    onSubmit() {
      this.$emit("search-text", this.text);
      this.text = "";
    }
  }
};
</script>

<style>
</style>