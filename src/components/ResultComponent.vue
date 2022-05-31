<template>

  <div class="results container-fluid">

    <div class="container text-center">

      <p class="text-uppercase pt-5">what are we doing</p>
      <h1 class="mb-5"><span id="results">Results</span> in Numbers</h1>

      <div class="row">
        <div class="col-3 my-5">
          <h1>128</h1>
          <h3>Certification</h3>
        </div>

        <div class="col-3 my-5">
          <h1>230</h1>
          <h3>Employees</h3>
        </div>

        <div class="col-3 my-5">
          <h1>517</h1>
          <h3>Customers</h3>
        </div>

        <div class="col-3 my-5">
          <h1>94</h1>
          <h3>Countries Served</h3>
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
  @import '../assets/style/mixins';

  .results {
    background: linear-gradient(
            rgba(0, 0, 0, 0.7), 
            rgba(0, 0, 0, 0.7)
    ),
    url(../assets/images/results.jpg);
    
    background-position: center;
    background-size: cover;
  }

  .container {
    padding: 105px 0px;

    h1, p {
      font-weight: bold;
      color: $white
    }

    p {
      color: $blue_lagoon;
    }

    #results {
      @include bg-text3();
    }
  }

  .col-3 {

    h1 {
      color: $blue_lagoon;
    }

    h3 {  
      color: $white;
      font-weight: bold;
    }
  }


</style>