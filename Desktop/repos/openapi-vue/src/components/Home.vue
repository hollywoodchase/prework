<template>
  <div class="hello">
    <h1>Whaddup</h1>
    <div id="add">
      {{ info }}
      {{ msg }}
      <h2>lalala</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {
    msg: String,
    info: String
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
