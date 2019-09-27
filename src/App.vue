<template>
  <div id="app">
    <div class="form-container">
      <Header msg="The Pamela Walsh Gallery"/>
      <Form question1='What is art?' question2='Why is art?'/>
    </div>
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
  html {
    background: url("./assets/painting-turner_rain.jpg") no-repeat center center fixed;
    background-color: rgb(249, 220, 126);
    background-size: cover;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 800px;
    width: 100%;
    text-align: center;
    margin: 0 auto;

  }
  .form-container {
    background-color: rgba(255, 255, 255, 0.8);
    border-style: ridge;
    border-width: 5px;
    border-color: rgba(84, 34, 1, 0.954);
    display: flex;
    flex-direction: column;
    width: fit-content;
    margin-bottom: 200px;
  }

  @media only screen and (min-width: 746px) {

  }
</style>
