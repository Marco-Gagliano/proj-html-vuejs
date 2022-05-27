<template>
  
  <div class="messagge container-fluid">
    <div class="container">
      <div class="row">

        <div class="col-6">
          <h6>send a messagge</h6>
          <h1>Get in touch</h1>
          <p>we will respond to your messagge as soon as possible</p>

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
              <input type="text" placeholder="More info">
            </div>

            <div class="col">
              <input type="text" placeholder="messagge">
            </div>

          </div>

        </div>  

        <div class="col-6">
          <h5>Example Inc.</h5>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
          <p>Praesent diam lacus, dapibus sed imperdit consectur.</p>
          <ul>
            <li>
              <i>TELEFONO  </i>
              <span>+1 (305) 1234-5678</span>
            </li>

            <li>
              <i>EMAIL  </i>
              <span>hello@spanle.com</span>
            </li>

            <li>
              <i>LUOGO  </i>
              <span>Main Avenue, 987</span>
              <button>VIEW MAP</button>
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

  .messagge {
    background-color: #FF1111;
    border: 1px solid #000000;
  }

  .container {
    background-color: #FFFFFF;
    border: 1px solid #000000;
  }

  .row {
    background-color: #D9FF00;
    border: 1px solid #000000;
  }

  .col, .col-6 {
    background-color: #00FF15;
    border: 1px solid #000000;
  }

</style>