<template>
  <basicIntro />
  <skill />
  <project />
  <workExp />
  <autobiography />
  <link />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import "./assets/scss/common.scss";
import basicIntro from "@/components/basicIntro.vue";
import skill from "@/components/skill.vue";
import workExp from "@/components/workExp.vue";
import project from "@/components/project.vue";
import autobiography from "@/components/autobiography.vue";
import link from "@/components/link.vue";

export default defineComponent({
  name: "App",
  components: { basicIntro, skill, workExp, project, autobiography, link },
  setup() {
    return {};
  },
});
</script>
