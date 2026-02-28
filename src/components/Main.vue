<script setup>
  import {ref} from 'vue'

  // array of facts about rin okumura
  // each fact has a highlight and description
  const arr = ref([
    {
      highlight: "good at cooking!",
      description: "Rin's cooking abilities won the respect of Ukobach, the stove spirit who prepares meals for Rin and Yukio."
    },
    {
      highlight: "a really cool dude!",
      description: "Rin is really strong, athletic, and is good at fighting. He also has a friendly personality."
    },
    {
      highlight: "empathetic.",
      description: "Rin is consistently able to empathize with other creatures and people that he's come across, just like his adoptive father, Shiro Fujimoto."
    }
  ])
</script>

<template>
  <main>
      <!-- renders one <section> for each fact in the array -->
      <!-- using v-for to iterate over the facts array automatically -->
      <section v-for="item in arr">
        <h2>
          He is <span class = "highlight">{{item.highlight}}</span>
        </h2>
        <p>
          {{item.description}}
        </p>
      </section>
  </main>
</template>

<style scoped>
  main {
    margin-top: 15px;
  }

  section {
    margin-top: 25px;
  }

  h2 {
    font-size: 1.3rem;
    color: #34495e;
    margin-bottom: 3px;
  }

  p {
    font-size: 0.9rem;
    color: #555;
  }
</style>