<template>
  <div class="skill">
    <p v-for="(skill, index) in skills" :key="index">{{ skill }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    let skills: string[] = [
      "HTML",
      "CSS",
      "JavaScript",
      "TypeScript",
      "Vue 2",
      "Vue 3",
      "ESlint",
      "Git",
      "Webpack",
      "D3.js",
      "Leaflet",
      "Element UI",
    ];
    return { skills };
  },
});
</script>
