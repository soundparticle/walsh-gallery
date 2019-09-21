<template>
  <div id="app">
    <!-- <img id="header-image" alt="Vue logo" src="./assets/logo.jpg"> -->
    <Header msg="Welcome to The Pamela Walsh Gallery"/>
    <Form question1='What is art?' question2='Why is art?'/>
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
  background-image: url("./assets/logo.jpg");
  background-size: contain;
  background-repeat: no-repeat;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 1000px;
  width: 1000px;
  text-align: center;
  margin-top: 60px;
  margin: 0 auto;
}
</style>
