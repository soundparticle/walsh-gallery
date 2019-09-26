<template>
  <div class="form">
    <form action="https://docs.google.com/forms/d/e/1FAIpQLSfA1sgQSFHpCWcXK6NMw0wS_oLOGqQeCFw3TaKp4xcgvtuGvQ/formResponse" target="_self" method="POST">
      <div class="form__body">
        <div class="form__question">
          <label class="form__label">{{ question1 }}</label>
          <input class="form__input" name="entry.668016936" />
        </div>
        <div class="form__question">
          <label class="form__label">{{ question2 }}</label>
          <input class="form__input" name="entry.1943360912" />
        </div>
        <button class="form__submit-button" type="submit">Submit</button>
      </div>
    </form>
  </div>
</template>

<script scoped>
export default {
  name: 'Form',
  props: {
    question1: String,
    question2: String,
  }
};
</script>

<style>
  form {
    /* display: flex; */
    /* justify-content: center; */
    font-family: 'Cinzel', serif;
  }
  .form__body {
    display: flex;
    flex-direction: column;
    /* width: 500px; */
    align-items: center;
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
    width: 300px;
  }
  .form__label {
    font-weight: bold;
    font-size: 20px;
  }
  .form__question {
    display: flex;
    flex-direction: column;
    margin: 50px 30px 0px 30px;
  }

  @media only screen and (min-width: 746px) {

    
  }
</style>
