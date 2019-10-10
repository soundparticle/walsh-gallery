<template>
<!-- possibly remove question props??? -->
  <div class="form">
    <form action="https://docs.google.com/forms/d/e/1FAIpQLSfA1sgQSFHpCWcXK6NMw0wS_oLOGqQeCFw3TaKp4xcgvtuGvQ/formResponse" target="_self" method="POST">
      <div class="form__body">
        <div class="form__question">
          <label class="form__label"></label>
          <input class="form__input" name="entry.668016936" v-model="input.name" placeholder="Name" autocomplete="off"/>
        </div>
        <div class="form__question">
          <label class="form__label"></label>
          <input class="form__input" name="entry.1943360912" v-model="input.address" placeholder="Address" autocomplete="off"/>
        </div>
        <div class="form__question">
          <label class="form__label"></label>
          <input class="form__input" name="entry.1338771678" v-model="input.email" placeholder="Email" autocomplete="off"/>
        </div>
        <button v-on:click="submit()" class="form__submit-button">Submit</button>
      </div>
    </form>
  </div>
</template>


<script scoped>
export default {
  name: 'Form',
  data() {
    return {
      input: {
        name: '',
        address: '',
        email: '',
      }
    };
  },
  methods: {
    submit() {
      // Maybe change conditional to be = , so it type matches???
      // refactor to ternary.
      if(this.input.name === '' || this.input.address === '' || this.input.email === '') {
        alert('You forgot something! Please fill out all fields.');
        event.preventDefault();
      }
      else return;
    }
  },
};
</script>


<style>
  form {
    font-family: 'Cinzel', serif;
  }
  .form__body {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 5px;
  }
  .form__submit-button {
    background-color: #000;
    color: #FFF;
    font-family: 'Cinzel', serif;
    margin-top: 50px;
    margin-bottom: 20px;
    padding: 10px;
    width: fit-content;
    align-content: center;
    font-size: 20px;
    font-weight: bold;
  }
  .form__input {
    margin-top: 10px;
    padding: 5px;
    width: 220px;
  }
  .form__label {
    font-weight: bold;
    font-size: 20px;
  }
  .form__question {
    display: flex;
    flex-direction: column;
    margin: 25px 30px 0px 30px;
  }

  @media only screen and (min-width: 746px) {

  }
</style>
