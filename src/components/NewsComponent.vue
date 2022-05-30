<template>

  <div class="news container-fluid">

    <div class="container py-5">

      <h6>our editorial content</h6>
      <h1 class="my-4">latest news</h1>

      <div class="d-flex justify-content-between">
        <p>Every week we publish content about what is best in the business world</p> 
        <button>SEE ALL</button>
      </div>

      <div class="row py-5">

        <div class="col-4">
        <img src="../assets/images/news-1.jpg" alt="">
          <h3 class="news-text-1">Increasing creativity is <br> possible for everyone</h3>
        </div>
        
        <div class="col-4">
        <img src="../assets/images/news-2.jpg" alt="">
          <h3 class="news-text-2">Because market <br> research is part of the <br> business plan</h3>
        </div>
        
        <div class="col-4">
        <img src="../assets/images/news-3.jpg" alt="">
          <h3 class="news-text-3">Working from home is <br> now a trend</h3>
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

  @import '../assets/style/vars';
  @import '../assets/style/mixins';

  .news {
    background-color: $gray_nurse;

    h6 {
      text-transform: uppercase;
      font-weight: bold;
      color: $blue_lagoon;
    }

    h1 {
      text-transform: capitalize;
      font-weight: bold;
      font-size: 58px;
    }

    p {
      font-size: 19px;
      color: $salt_box;
    }

    button {
      @include button_type1();
    }
  }

  .col-4 {

    img {
    width: 100%;
    border-radius: 5px;
    position: relative;
    background-color: $woodsmoke;
    }

    h3 {
      text-align: center;
      color: $woodsmoke;
      font-weight: bold;
    }

  }



</style>