<template>
  <div>
    <app-header :title="title"></app-header>
    <app-nijas :ninjas="ninjas"></app-nijas>
    <app-footer :copyright="copyright" :title="title"></app-footer>
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
      title: "VUE Ninjas",
      ninjas: [
        { name: "Ryu", speciality: "Kungfu", show: false },
        { name: "Karin", speciality: "Kyojutusu", show: false },
        { name: "Rock Lee", speciality: "Taijutusu", show: false },
        { name: "Naruto", speciality: "Ninjutsu", show: false },
        { name: "Sasuke", speciality: "Genjutsu", show: false },
        { name: "Itachi", speciality: "Genjutsu", show: false }
      ],
      copyright: "Copyright 2019"
    };
  },
  methods: {
    greeting: function() {
      return "hey wooop";
    },
    updateTitle: function(title) {
      this.title = title;
    }
  }
};
</script>

<style scoped>
h1 {
  color: purple;
}
</style>
