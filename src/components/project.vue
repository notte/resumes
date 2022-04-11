<template>
  <div class="project">
    <div class="item" v-for="(project, index) in projects" :key="index">
      <h3 class="name">{{ project.name }}</h3>
      <div class="img">
        <div></div>
        <div></div>
      </div>
      <button @click="clickLink(project.github)">Github</button>
      <button @click="clickLink(project.demo)">Demo</button>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    let projects = [
      {
        name: "TDX",
        img: ["...", "..."],
        github: "https://github.com/notte/tdx",
        demo: "https://github.com/notte/KKBOX_Demo",
      },
      {
        name: "Journey",
        img: ["...", "..."],
        github: "https://github.com/notte/HexWork",
        demo: "https://notte.github.io/HexWork/#/",
      },
      {
        name: "KKBOX_Demo",
        img: ["...", "..."],
        github: "https://github.com/notte/KKBOX_Demo",
        demo: "",
      },
    ];

    function clickLink(url: string): void {
      console.log(url);
    }
    return { projects, clickLink };
  },
});
</script>
