<template>
  <div class="form">
    <form @submit.prevent="handleSubmit" >
      <div class="form__body">
        <div class="form__question">
          <label class="form__label"></label>
          <input class="form__input" name="entry.280659687" v-model="contact.lastName" placeholder="Last Name" autocomplete="off"/>
        </div>
        <div class="form__question">
          <label class="form__label"></label>
          <input class="form__input" name="entry.668016936" v-model="contact.firstName" placeholder="First Name" autocomplete="off"/>
        </div>
        <div class="form__question">
          <label class="form__label"></label>
          <input class="form__input" name="entry.1943360912" v-model="contact.address" placeholder="Address" autocomplete="off"/>
        </div>
        <div class="form__question">
          <label class="form__label"></label>
          <input class="form__input" name="entry.1338771678" v-model="contact.email" placeholder="Email" autocomplete="off"/>
        </div>
        <button class="form__submit-button">Submit</button>
        <!-- <button v-on:click.prevent="submit()" class="form__submit-button">Submit</button> -->
      </div>
    </form>
  </div>
</template>


<script scoped>
export default {
  name: 'Form',
  data() {
    return {
      contact: Object.assign({}, this.contact)
    };
    // return {
    //   contact: {
    //     lastName: '',
    //     firstName: '',
    //     address: '',
    //     email: '',
    //   }
    // };
  },
  methods: {
    handleSubmit() {
      let contact = Object.assign({}, this.contact);
      console.log('contact', contact);
    },
    // refactor to ternary.

    // submit() {
    //   let contact = {};
    //   if(this.contact.lastName === '' || this.contact.lastName === '' || this.contact.address === '' || this.contact.email === '') {
    //     alert('You forgot something! Please fill out all fields.');
    //     //preventDefault() removed since was added to onClick method in submit button
    //     // event.preventDefault();
    //   }
    //   // else this.$router.push({ path: 'thank-you' });
    //   else return;
    // }
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
    border-radius: 5px;
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
