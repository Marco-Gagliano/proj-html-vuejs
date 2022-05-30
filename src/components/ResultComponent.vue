<template>

  <div class="results container-fluid">

    <div class="container text-center">

      <p class="text-uppercase pt-5">what are we doing</p>
      <h1 class="text-light mb-1">Results in Numbers</h1>

      <div class="row">
        <div class="col-3 my-5">
          <h2>128</h2>
          <p>Certification</p>
        </div>

        <div class="col-3 my-5">
          <h2>230</h2>
          <p>Employees</p>
        </div>

        <div class="col-3 my-5">
          <h2>517</h2>
          <p>Customers</p>
        </div>

        <div class="col-3 my-5">
          <h2>94</h2>
          <p>Countries Served</p>
        </div>

      </div>
    </div>
    
  </div>

</template>


<script>

export default {
  name: 'ResultComponent'
}
</script>


<style lang="scss" scoped>

  @import '../assets/style/vars';

  .results {
    background: linear-gradient(
            rgba(0, 0, 0, 0.7), 
            rgba(0, 0, 0, 0.7)
    ),
    url(../assets/images/results.jpg);
    
    background-position: center;
    background-size: cover;
  }

  h1, h2, p {
    font-weight: bold;
  }

  p {
    color: $blue_lagoon;
  }

  .col-3 h2 {
    color: $blue_lagoon;
  }
    
  .col-3 p {  
    color: $white;
  }

</style>