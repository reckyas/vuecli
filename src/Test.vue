<template>
  <div>
    <h1>List Of names</h1>
    <ul>
      <li v-for="(name, index) in names" :key="index">{{ name }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      names: ["yoshi", "yodha", "mario"]
    };
  }
};
</script>

<style scoped>
h1 {
  color: green;
}
</style>