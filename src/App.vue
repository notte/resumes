<template>
  <basicIntro />
  <skill />
  <project />
  <workExp />
  <autobiography />
  <connect />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import "./assets/scss/common.scss";
import basicIntro from "@/components/basicIntro.vue";
import skill from "@/components/skill.vue";
import workExp from "@/components/workExp.vue";
import project from "@/components/project.vue";
import autobiography from "@/components/autobiography.vue";
import connect from "@/components/connect.vue";

export default defineComponent({
  name: "App",
  // https://blog.build-school.com/2020/11/03/effective-resume/
  // https://tw.alphacamp.co/blog/2018-06-27-18378
  // eslint-disable-next-line vue/no-unused-components
  components: { basicIntro, skill, workExp, project, autobiography, connect },
  setup() {
    return {};
  },
});
</script>
