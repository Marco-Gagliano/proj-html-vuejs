<template>
  
  <div class="newsletter container-fluid">
    <div class="container">

      <div class="row">

        <div class="col-6">
          <h6>newsletter</h6>
          <h1>Know First</h1>
          <p>Follow closely and receive content about our company and the news of the current market</p>
        </div>

        <div class="col-6">
        <input type="text" name="" placeholder="Name">
        <input type="text" name="" placeholder="Email">
        <br>
        <button>SUBSCRIBE</button>
        </div>

      </div>

    </div>
  </div>

</template>


<script>

export default {
  name: 'NewsletterComponent'
}
</script>


<style lang="scss" scoped>

  .newsletter {
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