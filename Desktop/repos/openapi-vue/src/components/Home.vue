<template>
  <div class="hello">
    <h1>Whaddup</h1>
  </div>
</template>

<script>
import OpenAPIClientAxios from "openapi-client-axios";

async () => {
  const api = new OpenAPIClientAxios({
    definition:
      "https://raw.githubusercontent.com/OAI/OpenAPI-Specification/master/examples/v3.0/petstore.yaml",
  });
  const client = await api.init();
  const res = await api.getPets(); // res.data will contain the result of the API call
  console.log(res);
  console.log(client);

};

export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
