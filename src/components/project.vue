<template>
  <div class="project">
    <div class="item">
      <h3 class="name">TDX</h3>
      <div class="img">
        <div></div>
        <div></div>
      </div>
      <button>Github</button>
      <button>Demo</button>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    let projects = [
      { name: "TDX", img: ["...", "..."], github: "...", demo: "..." },
    ];
    return { projects };
  },
});
</script>
