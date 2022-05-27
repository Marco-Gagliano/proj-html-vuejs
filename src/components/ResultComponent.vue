<template>

  <div class="results container-fluid">

    <div class="container text-center">

      <p>what are we doing</p>
      <h1>results in numbers</h1>

      <div class="row">
        <div class="col-3">
          <p>128</p>
          <p>Certification</p>
        </div>

        <div class="col-3">
          <p>230</p>
          <p>Employees</p>
        </div>

        <div class="col-3">
          <p>517</p>
          <p>Customers</p>
        </div>

        <div class="col-3">
          <p>94</p>
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

  .container {
    background-color: #FFFFFF;
    border: 1px solid #000000;
  }

  .results {
    background-color: #FF1111;
    border: 1px solid #000000;
  }

  .row {
    background-color: #D9FF00;
    border: 1px solid #000000;
  }

  .col-3 {
    background-color: #00FF15;
    border: 1px solid #000000;
  }

</style>