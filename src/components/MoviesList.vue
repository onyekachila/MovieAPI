<template>
  <div>{{movie.id}}</div>
</template>

<script>
export default {
  name: "MoviesList",
  data() {
    return {
      movie: {}
    };
  },
  created: function() {
    this.fectchData();
  },
  methods: {
    fectchData: async function() {
      try {
        const res = await fetch(
          "https://api.themoviedb.org/3/movie/550?api_key=6fe4e2cd9edc107dd7d61509d3d05de3"
        );
        const movie = await res.json();
        this.movie = movie;
      } catch (e) {
        console.log(e);
      }
    }
  }
};
</script>


<style scoped>
</style>
