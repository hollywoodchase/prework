<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Home 
      msg="Welcome to Your Vue.js App"
      info=""
    />
  </div>
</template>


<script>
 const vm = new Vue({
        el: '#app',
        //Mock data for the value of BTC in USD
        data: { BTCinUSD: 3759.91, BTCinEURO:3166.21 }
      });

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
