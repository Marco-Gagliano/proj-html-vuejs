<template>
  
  <footer class="container-fluid">
    <div class="container">
      <div class="row">

        <div class="col-3">
          <h4>nexgen</h4>
          <p>A Functional HTML Template for Corporate & Business.</p>
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
            </li>
            
            <button>GET IN TOUCH</button>
          </ul>

        </div>

        <div class="col-3">

          <h1>About</h1>
          <ul>
            <li><a href="#">The Company</a></li>
            <li><a href="#">Institutional</a></li>
            <li><a href="#">Social & Events</a></li>
            <li><a href="#">Innovation</a></li>
            <li><a href="#">Environment</a></li>
            <li><a href="#">Technology</a></li>
          </ul>
        </div>

        <div class="col-3">
        
          <h1>Services</h1>
          <ul>
            <li><a href="#">Audit & Assurance</a></li>
            <li><a href="#">Financial Advisory</a></li>
            <li><a href="#">Analytics M&A</a></li>
            <li><a href="#">Middle Marketing</a></li>
            <li><a href="#">Legal Consulting</a></li>
            <li><a href="#">Regulatory Risk</a></li>
          </ul>
        </div>

        <div class="col-3">
        
          <h1>Support</h1>
          <ul>
            <li><a href="#">Responsibility</a></li>
            <li><a href="#">Terms of Use</a></li>
            <li><a href="#">About Cookies</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li><a href="#">Accessibility</a></li>
            <li><a href="#">Information</a></li>
          </ul>
        </div>
        
      </div>

      <div class="row">

        <div class="col-6"> 
          <p>Enjoy the low price. We are Tracking any intention of piracy</p>
        </div>

        <div class="col-6">
          <p>@2020 NEXGEN is Proudly Powered by Codings.</p>
        </div>
      </div>

    </div>

  
  </footer>

</template>


<script>

export default {
  name: 'FooterComponent'

}
</script>


<style lang="scss" scoped>

  footer {
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

  .col, .col-3 {
    background-color: #00FF15;
    border: 1px solid #000000;
  }

</style>