<template>
  <div id="form-container">
    <h1>Please fill our form..</h1>
    <div id="form-header">
      <slot name="form-header"></slot>
    </div>
    <div id="form-fields">
      <slot name="form-fields"></slot>
    </div>
    <div id="form-controls">
      <slot name="form-controls"></slot>
    </div>
    <div id="useful-links">
      <ul>
        <li>
          <a href="#">Link 1</a>
        </li>
        <li>
          <a href="#">Link 2</a>
        </li>
        <li>
          <a href="#">Link 3</a>
        </li>
        <li>
          <a href="#">Link 4</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {};
  },
  methods: {}
};
</script>

<style scoped>
#form-container {
  width: 100%;
  max-width: 960px;
  margin: 0 auto;
}
#form-header,
#form-fields,
#form-controls,
#useful-links {
  padding: 10px;
  margin: 10px 0;
  background: #ccc;
}
#form-header {
  text-align: center;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  color: #111;
}
#form-fields {
  display: flex;
  text-align: center;
}
#useful-links {
  text-align: center;
}
#useful-links ul {
  list-style-type: none;
  display: flex;
  padding: 0;
  width: 100%;
  justify-content: center;
}
#useful-links ul li {
  padding: 10px;
}
</style>
