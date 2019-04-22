<template>
  <footer>
    <p>{{ copyright }} {{ title }}</p>
  </footer>
</template>

<script>
export default {
  props: {
    copyright: {
      type: String
    },
    title: {
      type: String
    }
  },
  data() {
    return {};
  }
};
</script>

<style scoped>
footer {
  background: #222;
  padding: 10px;
}
p {
  color: lightgreen;
  text-align: center;
}
</style>
