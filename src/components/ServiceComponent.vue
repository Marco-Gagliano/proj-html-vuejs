<template>

  <div class="service container-fluid py-5">

    <div class="container">

      <div class="info-service">

        <h6 class="text-uppercase pt-5">our business areas</h6>
        <h1>Excellent in Services</h1>

        <div class="row my-4">

          <div class="col-7">
            <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.</p>
          </div>

          <div class="col-5">
            <button>SEE ALL</button>
          </div>

        </div>
        
      </div>

      <div class="description-service">
        <div class="row justify-content-between">

          <div class="col">
            <i>icona</i>
            <i class="fa-solid fa-arrow-right"></i>
            <h5>Audit & Assurance</h5>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
          </div>
          
          <div class="col">
            <i class="fa-regular fa-briefcase"></i>
            <i class="fa-solid fa-arrow-right"></i>
            <h5>Financial Advisory</h5>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
          </div>
          
          <div class="col">
            <i class="fa-regular fa-chart-simple"></i>
            <a href="#"><i class="fa-solid fa-arrow-right"></i></a>
            <h5>Analytics and M&A</h5>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
          </div>
        </div>  
          
        <div class="row justify-content-between">
          <div class="col">
            <i>icona</i>
            <a href="#"><i class="fa-solid fa-arrow-right"></i></a>
            <h5>Middle Marketing</h5>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
          </div>
          
          <div class="col">
            <i class="fa-solid fa-globe-stand"></i>
            <a href="#"><i class="fa-solid fa-arrow-right"></i></a>
            <h5>Legal Consulting</h5>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
          </div>
          
          <div class="col">
            <i>icona</i>
            <a href="#"><i class="fa-solid fa-arrow-right"></i></a>  
            <h5>Regulatory Risk</h5>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>  
          </div>

        </div>
      </div>

    </div>

  </div>

</template>


<script>

export default {
  name: 'BusinessComponent'

}
</script>


<style lang="scss" scoped>

  .service {
    background-color: #111117;
  }

  h1, h5, h6 {
    font-weight: bold;
  }

  h6 {
    color: #048383
  }

  h1 {
    color: #FFFFFF
  }

  p {
    color: #BCBDBD
  }


  // INFO SERVICE

  .info-service h1 {
    font-size: 52px;
  }

  .col-5 button {
    float: right;
    margin: 0 10px;
    background-color: rgba($color: #000000, $alpha: 0);
    color: #FFFFFF;
    border: none;
    border: 1px solid #048383;
    border-radius: 5px;
    padding: 8px 30px;
  }  

  // /INFO SERVICE


  // DESCRIPTION SERVICE

  h5 {
    padding: 10px 0;
  }

  .description-service h5 {
    color: #FFFFFF
  }

  .description-service .col {
    background-color: #1D2528;
    margin: 15px;
    padding: 30px 50px;
    border-radius: 7px;
  }

  .description-service i {
    color: #048383;
  }

  .description-service .fa-arrow-right {
    float: right;
    font-size: 24px;
    color: #098081;
  }
  // /DESCRIPTION SERVICE

</style>