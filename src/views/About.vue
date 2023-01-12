<template>
  <div class="about">
    <h1>About</h1>
    
    <p>TODO Application with Vue js created by students at ISET Djerba</p>

    <transition name="fade">
      <div v-if="showP">bonjour, L3MDW</div>
    </transition>
    <button @click="showP = !showP"> click me </button>
  </div>
</template>

<script>



import { ref } from 'vue'

export default {

  setup() {
    const showP = ref(false)
    return { showP }
  }
}

</script>

<style>
  .about {
    max-width: 600px;
    margin: 20px auto;
  }

   .fade-enter-from {
    opacity: 0;
  }
  .fade-enter-to {
    opacity: 1;
  }
  .fade-enter-active {
    transition: all 2s ease;
  }
  .fade-leave-from {
    opacity: 1;
  }
  .fade-leave-to {
    opacity: 0;
  }
  .fade-leave-active {
    transition: all 2s ease;
  }
</style>