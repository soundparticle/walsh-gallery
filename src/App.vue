<template>
  <div id="app">
    <img id="header-image" alt="Vue logo" src="./assets/logo.jpg">
    <Header msg="Welcome to The Pamela Walsh Gallery"/>
    <Form question1="What is art?" question2="Why is art?"/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Form from './components/Form.vue';

export default {
  name: 'app',
  components: {
    Header,
    Form
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#header-image {
  max-width: 1000px;
}

</style>
