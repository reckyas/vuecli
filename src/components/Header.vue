<template>
  <header>
    <h1 @click="changeTitle">{{ title }}</h1>
  </header>
</template>

<script>
import { bus } from "../main";
export default {
  props: {
    title: {
      type: String
    }
  },
  data() {
    return {};
  },
  methods: {
    changeTitle: function() {
      // this.$emit("changeTitle", "VUE wizard");
      this.title = "Vue Wizards";
      bus.$emit("titleChanged", "View Wizard");
    }
  }
};
</script>

<style scoped>
header {
  background: lightgreen;
  padding: 10px;
}
h1 {
  text-align: center;
  color: #222;
}
</style>
