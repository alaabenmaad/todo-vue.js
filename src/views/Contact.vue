<template>
  <div class="contact">
    <h1>Team</h1>
    <ul>
      <li >
        <span class="material-icons">account_circle</span>
        <div>Alaa Eddine BEN MAAD</div>
        <a target="_blank" href="https://alaa-benmaad.me/">website</a>
      </li>

      <li >
        <span class="material-icons">account_circle</span>
        <div>Bilel BEN YOUSSEF</div>
        <a target="_blank" href="https://bilelbenyoussef.me/">website</a>
      </li>

      <li >
        <span class="material-icons">account_circle</span>
        <div> Wieme MESTAOUI</div>
        <a target="_blank" href="https://mo3dli.tn/">website</a>
      </li>
    </ul>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const icons = ref([
      { name: 'account_circle', text: 'Alaa BEN MAAD'},
      { name: 'account_circle', text: 'Bilel BEN YOUSSEF'},
      { name: 'account_circle', text: 'Wieme MESTAOUI'},
    ])

    return { icons }
  }
}
</script>

<style>
  .contact ul {
    padding: 0;
    display: grid;
    grid-template-columns: 2fr ;
    grid-gap: 20px;
    max-width: 400px;
    margin: 60px auto;
  }
  .contact li {
    list-style-type: none;
    background: white;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 1px 3px 5px rgba(0,0,0,0.1);
    cursor: pointer;
    line-height: 1.5em;
  }
</style>