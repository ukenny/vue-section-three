<template>
  <div class="hello">
    <p v-show="show">Now you see me!</p>
    <p v-show="!show">Now you don't!</p>
    <button @click="show = !show">Switch</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data: function() {
    return { show: Boolean };
  },
  created: function() {
    this.show = false;
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
