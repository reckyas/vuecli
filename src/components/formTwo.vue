<template>
  <div>
    <form-helper>
      <div slot="form-header">
        <h1>Comment form</h1>
        <p>Information for form</p>
      </div>
      <div slot="form-fields">
        <input type="text" placeholder="name">
        <textarea cols="30" rows="10"></textarea>
      </div>
      <div slot="form-controls">
        <button>Submit</button>
      </div>
    </form-helper>
  </div>
</template>

<script>
import formHelper from "./formHelper";
export default {
  components: {
    "form-helper": formHelper
  },
  data() {
    return {};
  }
};
</script>
