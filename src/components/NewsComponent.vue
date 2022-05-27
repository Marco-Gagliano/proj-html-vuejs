<template>

  <div class="news container-fluid">

    <div class="container">

      <h6>our editorial content</h6>
      <h1>latest news</h1>
      <div class="d-flex justify-content-between">
        <p>Every week we publish content about what is best in the business world</p> 
        <button>SEE ALL</button>
      </div>

      <div class="row">

        <div class="col-4">
          <h1>IMMAGINE</h1>
          <p>Increasing creativity is possible for everyone</p>
        </div>
        
        <div class="col-4">
          <h1>IMMAGINE</h1>
          <p>Because market research is part of the business plan</p>
        </div>
        
        <div class="col-4">
          <h1>IMMAGINE</h1>
          <p>Working from home is now a trend</p>
        </div>

      </div>
      
    </div>
  </div>

</template>


<script>

export default {
  name: 'NewsComponent'
}
</script>


<style lang="scss" scoped>

  .news {
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

  .col, .col-4 {
    background-color: #00FF15;
    border: 1px solid #000000;
  }


</style>