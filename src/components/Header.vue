<template>
  <div class="header">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
  export default {
    name: 'Header',
    props: {
      msg: String
    },
  };
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1 {
    font-family: 'Cinzel', serif;
    font-size: 24px;
    padding: 10px;
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

  @media only screen and (min-width: 746px) {


  }
</style>
