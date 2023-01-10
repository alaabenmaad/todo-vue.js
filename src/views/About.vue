<template>
  <div class="about">
    <h1>About</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aperiam officia possimus delectus inventore quod quisquam culpa voluptas iusto, quae maiores quo dolorum, corporis laboriosam a dolore consequatur assumenda nam!</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aperiam officia possimus delectus inventore quod quisquam culpa voluptas iusto, quae maiores quo dolorum, corporis laboriosam a dolore consequatur assumenda nam!</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum aperiam officia possimus delectus inventore quod quisquam culpa voluptas iusto, quae maiores quo dolorum, corporis laboriosam a dolore consequatur assumenda nam!</p>

    <transition name="fade">
      <div v-if="showP">hello, L3MDW</div>
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