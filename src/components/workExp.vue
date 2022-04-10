<template>
  <div class="workExp">
    <div class="item" v-for="(work, index) in works" :key="index">
      <p class="time">{{ work.time }}</p>
      <h3 class="name">{{ work.name }}</h3>
      <h4 class="company">{{ work.company }}</h4>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    interface IWork {
      name: string;
      company: string;
      time: string;
    }
    let works: IWork[] = [
      {
        name: "網頁設計師",
        company: "星爵科技",
        time: "2019-03 至今",
      },
      {
        name: "網頁設計師",
        company: "奕兆有限公司",
        time: "2017-12 至 2019-02",
      },
      {
        name: "網頁設計師",
        company: "歐萊德",
        time: "2017-04 至 2017-11",
      },
      {
        name: "網頁設計師",
        company: "首岳資訊",
        time: "2017-02 至 2017-04",
      },
      {
        name: "遊戲介面美術",
        company: "八樂數位科技",
        time: "2016-07 至 2016-12",
      },
      { name: "遊戲介面美術", company: "中華網龍", time: "2013-06 至 2016-07" },
    ];
    return { works };
  },
});
</script>
