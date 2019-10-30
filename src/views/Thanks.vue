<template>
  <div id="app">
    <h1>This is the thank you page</h1>
    <p>Thank you for signing up!</p>
      <router-link to="/">Back To Form</router-link>
  </div>
</template>

<script>
export default {
  name: 'Thanks',
};

</script>

<style scoped>
  #app {
    background-color: rgba(255, 255, 255, 0.8);
    border-radius: 10px;
    border-style: ridge;
    border-width: 5px;
    border-color: rgba(84, 34, 1, 0.954);
    padding: 15px;
  }
</style>
