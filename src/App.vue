<script setup>
  import Button from './components/Button.vue'
  import ButtonCounter from './components/ButtonCounter.vue';
    
</script>

<template>
  <div class="container mx-auto">
    <div class="flex items-center mt-5">
      <img class="logo" src="./assets/vue.svg" alt="Vue logo" />
      <h1 class="text-2xl">Vue Components</h1>
    </div>
    <div class="mt-10 p-10">
      <p class="mb-3">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis corporis mollitia fugit dolor quibusdam atque qui fuga laudantium aut porro.
      </p>

      <!-- without props having default values -->
      <Button/>


      <!-- with props with given value -->
      <Button label="Click Me" color="orange" class="ml-5"/>
      <Button label="Again Click Me" color="red" class="ml-5"/>

    </div>


    <div class="mt-10 p-10">
      <p class="mb-3">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis corporis mollitia fugit dolor quibusdam atque qui fuga laudantium aut porro.
      </p>


      <!-- ButtonCouter Component -->
      <ButtonCounter start="20"/>

      <br><br>

      <button-counter/>


    </div>
    
  </div>
    
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
