<template>
  
  <div class="messagge container-fluid">
    <div class="container">
      <div class="row send-messagge">

        <div class="col-6 my-5">

          <h6>send a messagge</h6>
          <h1 class="my-4">Get in Touch</h1>
          <p class="my-4">We will respond to your messagge as soon as possible.</p>

          <div class="row">

            <div class="col-6">
              <input type="text" placeholder="Name">
            </div>

            <div class="col-6">
              <input type="text" placeholder="Email">
            </div>
            

            <div class="col-6">
              <input type="text" placeholder="Phone">
            </div>

            <div class="col-6">
              <input type="text" placeholder="More Info">
            </div>

            <div class="col-12">
              <input type="text" placeholder="Messagge" class="messagge">
            </div>

            <div class="col mt-3">
              <button>SEND</button>
            </div>

          </div>

        </div>  

        <div class="contact-messagge col-6 my-5">

          <h4 class="fw-bold">Example Inc.</h4>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          <p>Praesent diam lacus, dapibus sed imperdit consectur.</p>

          <ul>
            <li>
              <i class="fa-solid fa-phone"></i>
              <span>+1 (305) 1234-5678</span>
            </li>

            <li>
              <i class="fa-solid fa-envelope"></i>
              <span>hello@example.com</span>
            </li>

            <li>
              <i class="fa-solid fa-location-dot"></i>
              <span>Main Avenue, 987</span>
            </li>

            <li>
              <button class="button-map">VIEW MAP</button>
            </li>
          </ul>
          
        </div>  

      </div>
    </div>
  </div>

</template>


<script>

export default {
  name: 'MessaggeComponent'
}
</script>


<style lang="scss" scoped>

  @import '../assets/style/vars';
  @import '../assets/style/mixins';

  .send-messagge {

    h6 {
      color: $blue_lagoon;
      text-transform: uppercase;
      font-weight: bold;
    }

    h1 {
      font-weight: bold;
    }

    p {
      color: $salt_box;
    }

    input {
      background-color: $gray_nurse;
      border: 0;
      margin-bottom: 10px;
      padding: 10px;
      border-radius: 5px;
      width: 100%;
    }

    ul {
      padding: 0;

      li {
        padding-bottom: 15px;
      }
    }

    .messagge {
      padding-bottom: 100px
    }

    button {
      @include button_type1();
    }

    .button-map {
      @include button_type3();
    }
  }

  .contact-messagge {
    color: $salt_box;
    padding-left: 35px;

    h4 {
      color: $shark;
    }

    p {
      padding-right: 273px;
    }

    i {
      color: $blue_lagoon;
      background-color: $gray_nurse;
      padding: 12px;
      margin-right: 15px;
      font-size: 18px;
      border-radius: 100px;
    }
  }

</style>