<template>
  <div id="ninjas">
    <ul>
      <li v-for="(ninja, index) in ninjas" :key="index" @click="ninja.show=!ninja.show">
        <h2>{{ ninja.name }}</h2>
        <h3 v-show="ninja.show">{{ ninja.speciality }}</h3>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ninjas: [
        { name: "Ryu", speciality: "Kungfu", show: false },
        { name: "Karin", speciality: "Kyojutusu", show: false },
        { name: "Rock Lee", speciality: "Taijutusu", show: false },
        { name: "Naruto", speciality: "Ninjutsu", show: false },
        { name: "Sasuke", speciality: "Genjutsu", show: false },
        { name: "Itachi", speciality: "Genjutsu", show: false }
      ]
    };
  }
};
</script>

<style>
#ninjas {
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
}
ul {
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  padding: 0;
}
li {
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 30px;
  border: 1px solid #222;
  margin: 10px;
  cursor: pointer;
}
</style>
