<template>
  
  <div class="newsletter container-fluid">
    <div class="container py-5">

      <div class="row">

        <div class="col-6">
          <h6>newsletter</h6>
          <h1 class="my-3"><span id="know">Know</span> First</h1>
          <p>Follow closely and receive content about our company and the news of the current market.</p>
        </div>

        <div class="col-6">
          <input v-model.trim="nameForm" type="text" name="yout_name" placeholder="Name">
          <input v-model.trim="emailForm" type="email" name="your_email" placeholder="Email">
          <br>
          <button @click="sendNewsletter()">SUBSCRIBE</button>
          <h4>{{confirm}}</h4>
        </div>

      </div>

    </div>
  </div>

</template>


<script>

export default {
  name: 'NewsletterComponent',

  data() {
    return {
      nameForm: '',
      emailForm: '',
      confirm: ''
    }
  },

  methods: {
    sendNewsletter(){
      this.$emit( this.nameForm , this.emailForm );
      this.nameForm = '';
      this.emailForm = '';
      this.confirm = '*Registrazione Confermata';
    },
  }
}
</script>


<style lang="scss" scoped>

  @import '../assets/style/vars';
  @import '../assets/style/mixins';

  .newsletter {
    background-color: $woodsmoke;
    padding: 100px 0px;

    .container {
      padding: 0px 120px;
    }

    h1 {
      color: $white;
      font-weight: bold;

      #know {
        @include bg-text3();
      }
    }

    h4 {
      color: $blue_lagoon;
    }

    h6 {
      color: $blue_lagoon;
      font-weight: bold;
      text-transform: uppercase;
    }

    p {
      padding-right: 140px;
      color: $silver_sand;
    }
  }

  .col-6 {
    
    input {
      margin-bottom: 10px;
      width: 60%;
      padding: 10px;
      border-radius: 5px;
      border: 0;
      background-color: $shark;
      color: $silver_sand;
    }

    button {
      @include button_type1();
    }
  }

</style>