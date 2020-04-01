<template>
  <div class=" section">
        <h1 class="brand-index">
         <span>funny</span><br>
         <span>dad</span><br>
         <span>jokes</span>
        </h1>
      
    <h3>Welcome to your daily dose of embarrassment</h3>
    <img src="../static/kingdom-3.png" alt="Illustration" class="img-fluid">
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
