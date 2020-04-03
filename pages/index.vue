<template>
  <div class="section">
     <div class="section-title float-left">
        <h1 class="brand-index">
          <span>funny</span><br>
          <span>dad</span><br>
          <span>jokes</span>
        </h1>
     <h2>Welcome to your daily dose of embarrassment!</h2>
    </div>

        <img src="../static/kingdom-3.png" alt="Illustration" class="section-img float-right">
  </div>
</template>

<script>
export default {
    head(){
        return {
            title: 'Funny Dad Jokes',
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
