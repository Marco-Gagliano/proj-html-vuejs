<template>
  
  <footer class="container-fluid">
    <div class="contacts container-fluid py-5">
      <div class="container py-5">
        <div class="row">

          <div class="col-3 info">
            <ul>
              <li>
                <h4>nexgen</h4>          
              </li>
              
              <li>
                <p>A Functional HTML Template for Corporate & Business.</p>
              </li>
            
              <li>
                <i class="fa-solid fa-phone"></i>
                <span>+1 (305) 1234-5678</span>
              </li>

              <li>
                <i class="fa-solid fa-envelope"></i>
                <span>hello@spanle.com</span>
              </li>

              <li>
                <i class="fa-solid fa-location-dot"></i>
                <span>Main Avenue, 987</span>
              </li>

              <li>
                <button>GET IN TOUCH</button>           
              </li>
            </ul>

          </div>

          <div class="col-3 contact">

            <ul>
              <li><h3>About</h3></li>

              <li>  
                <a href="#"><i class="fa-solid fa-chevron-right"></i>

                The Company</a>
              </li>

              <li>  
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Institutional</a>
              </li>

              <li>  
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Social & Events</a>
              </li>

              <li>  
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Innovation</a>
              </li>

              <li>  
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Environment</a>
              </li>

              <li>  
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Technology</a>
              </li>

            </ul>
          </div>

          <div class="col-3 contact">
          
            <ul>
              <li><h3>Services</h3></li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Audit & Assurance</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Financial Advisory</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Analytics M&A</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Middle Marketing</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Legal Consulting</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Regulatory Risk</a>
              </li>

            </ul>

          </div>

          <div class="col-3 contact">
          
            <ul>
              <li><h3>Support</h3></li>
              
              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Responsibility</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Terms of Use</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                About Cookies</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Privacy Policy</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Accessibility</a>
              </li>

              <li>
                <a href="#"><i class="fa-solid fa-chevron-right"></i>
                Information</a>
              </li>

            </ul>
          </div>
          
        </div>

      </div>
    </div>

    <div class="credits container-fluid">
      <div class="container">
        <div class="row d-flex align-items-center">

          <div class="col-6"> 
            <p>Enjoy the low price. We are Tracking any intention of piracy</p>
          </div>

          <div class="col-6 d-flex justify-content-end align-items-center">
            <p>@2020 NEXGEN is Proudly Powered by Codings.</p>
          </div>

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
    padding: 0;
  }

  .contacts {
    background-image: url(../assets/images/bg-7.jpg);
    background-position: center;
    color: #BCBDBD;
  }

  .info {
    ul {
      padding: 0;
    }

  }


  h4 {
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 5px;
  }

  h3 {
    font-weight: bold;
    color: #E7EEEA;
  }

  p {
    padding-right: 80px;
  }


  i {
    padding-right: 10px;
  }
  
  button {
    background: none;
    color: #FFFFFF;
    border: none;
    border: 1px solid #048383;
    border-radius: 5px;
    padding: 8px 30px;
    margin: 15px 0;
  }

  .contact {
    display: flex;
    align-items: center;
    background-color: rgba($color: #1D2528, $alpha: 0.4);
    border-radius: 10px;
    margin-right: 30px;
    width: calc(100% / 5);
  }
  


  .credits {
    color: #BCBDBD;
    background-color: #111117;
    

  }

    .col-6 {
      float: right;
    }
</style>