<template>
  <div class=" section">
     <div class="flex">
        <h1 class="brand-index">
          <span>funny</span><br>
          <span class="blue">dad</span><br>
          <span class="yellow">jokes</span>
        </h1>

        <img src="../static/kingdom-3.png" alt="Illustration" class="img-fluid">
    </div>
     <h3>Welcome to your daily dose of embarrassment</h3>
  </div>
</template>

<script>
export default {
    head(){
        return {
            title: 'Welcome to Dad Jokes!',
            meta: [ {
                hid:'description',
                name: 'description',
                content: 'Welcome to Dad Jokes!'
               }
            ]
        }
    }
}
</script>
