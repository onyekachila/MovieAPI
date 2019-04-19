<template>
  <div>
    <header>
      <h1>{{title}}</h1>
    </header>
  </div>
</template>


<script>
export default {
  props: {
    title: String
  },
  name: "Header"
};
</script>


<style scoped>
header {
  background-color: #111;
  padding: 20px;
  color: white;
}
h1 {
  margin: 0;
}
</style>
