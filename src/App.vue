<template>
  <div>
    <app-header></app-header>
    <app-nijas></app-nijas>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Ninjas from "./components/Ninjas.vue";
export default {
  components: {
    "app-header": Header,
    "app-footer": Footer,
    "app-nijas": Ninjas
  },
  data() {
    return {
      title: "Aplikasi dengan file vue pertama saya"
    };
  },
  methods: {
    greeting: function() {
      return "hey wooop";
    }
  }
};
</script>

<style scoped>
h1 {
  color: purple;
}
</style>
