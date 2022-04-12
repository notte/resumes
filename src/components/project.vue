<template>
  <div class="project">
    <div class="item">
      <h3 class="name">TDX</h3>
      <div class="img">
        <div class="size">
          <img src="../assets/project1-1.png" alt="" />
        </div>
        <div class="size">
          <img src="../assets/project1-2.png" alt="" />
        </div>
      </div>
      <button @click="clickLink('https://github.com/notte/tdx')">Github</button>
      <button @click="clickLink('https://github.com/notte/KKBOX_Demo')">
        Demo
      </button>
    </div>
    <div class="item">
      <h3 class="name">Journey</h3>
      <div class="img">
        <div class="size">
          <img src="../assets/project2-1.png" alt="" />
        </div>
        <div class="size">
          <img src="../assets/project2-2.png" alt="" />
        </div>
      </div>
      <button @click="clickLink('https://github.com/notte/HexWork')">
        Github
      </button>
      <button @click="clickLink('https://notte.github.io/HexWork/#/')">
        Demo
      </button>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    function clickLink(url: string): void {
      console.log(url);
    }
    return { clickLink };
  },
});
</script>
