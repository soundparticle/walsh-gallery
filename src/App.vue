<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/thank-you">Thanks</router-link>
    </div>
    <router-view/>
  </div>
</template>

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
    overflow: hidden;

  }
  .form-container {
    background-color: rgba(255, 255, 255, 0.8);
    border-style: ridge;
    border-width: 5px;
    border-color: rgba(84, 34, 1, 0.954);

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    width: 85vw;
    margin-left: 20px;
    margin-right: 20px;
    margin-top: 60px;
    margin-bottom: 200px;
  }

  @media only screen and (min-width: 746px) {
    .form-container {
      width: 500px;
    }
  }
</style>
