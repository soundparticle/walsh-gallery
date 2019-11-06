<template>
  <div class="header">
    <!-- <h1>The Pamela Walsh Gallery</h1> -->
    <img src="../assets/PWG-logo-horizontal.jpg">
  </div>
</template>

<script>
export default {
  name: 'Header',
};
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1 {
    font-family: 'Cinzel', serif;
    font-size: 24px;
    padding: 5px;
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

  img {
    height: 100px;
    padding-top: 40px;
  }

  @media only screen and (min-width: 746px) {

  }
</style>
