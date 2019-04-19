<template>
  <div id="app">
    <Header :title="title"/>

    <MoviesList/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import MoviesList from "./components/MoviesList.vue";

export default {
  name: "app",
  data() {
    return {
      hello: "Hello From Data",
      title: "Vue Movie DB",
      isTrue: false
    };
  },
  components: {
    Header,
    MoviesList
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
}
</style>

