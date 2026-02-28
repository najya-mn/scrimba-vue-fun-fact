<!-- footer component -->
<script setup>
import {ref} from 'vue'
//  reactive reference to the external link for Rin Okumura's Wikia page
const href = ref("https://aonoexorcist.fandom.com/wiki/Rin_Okumura")
</script>

<template>
  <footer>
      <!-- footer credit/text with a link that opens in a new tab -->
      <!-- using v-bind shorthand ':href' to dynamically bind the ref -->
      <p>Learn more about Rin Okumura at his <a target="_blank" :href>Wikia page</a>!</p>
  </footer>
</template>

<style scoped>
  footer {
    margin-top: 35px;
    font-size: 0.8rem;
  }
  a {
    color: rgb(61, 123, 255);
  }
</style>