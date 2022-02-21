<template>
  <basicIntro />
  <skill />
  <workExp />
  <project />
  <autobiography />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import "./assets/scss/common.scss";
import basicIntro from "@/components/basicIntro.vue";
import skill from "@/components/skill.vue";
import workExp from "@/components/workExp.vue";
import project from "@/components/project.vue";
import autobiography from "@/components/autobiography.vue";

export default defineComponent({
  name: "App",
  components: { basicIntro, skill, workExp, project, autobiography },
  setup() {
    return {};
  },
});
</script>
