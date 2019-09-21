<template>
  <div class="form">
    <form action="https://docs.google.com/forms/d/e/1FAIpQLSfA1sgQSFHpCWcXK6NMw0wS_oLOGqQeCFw3TaKp4xcgvtuGvQ/formResponse" target="_self" method="POST">
      <div class="form__container">
        <label class="form__name">{{ question1 }}</label>
        <input class="form__input" name="entry.668016936" />
        <label class="form__name">{{ question2 }}</label>
        <input class="form__input" name="entry.1943360912" />
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
  display: flex;
  justify-content: center;
}
.form__container {
  display: flex;
  flex-direction: column;
  width: 500px;
}

.form__submit-button {
  background-color: #000;
  color: #FFF;
}
</style>
