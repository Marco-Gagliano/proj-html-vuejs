<template>

  <div class="news container-fluid">

    <div class="container">

      <h6>our editorial content</h6>
      <h1 class="my-4">latest <span id="news">news</span></h1>

      <div class="d-flex justify-content-between">
        <p>Every week we publish content about what is best in the business world</p> 
        <button>SEE ALL</button>
      </div>

      <div class="row py-5">

        <div class="col-4 left">
          <img src="../assets/images/news-1.jpg" alt="">
          <h3 class="news-text-1">Increasing creativity is <br> possible for everyone</h3>
        </div>
        
        <div class="col-4 middle">
          <img src="../assets/images/news-2.jpg" alt="">
          <h3 class="news-text-2">Because market <br> research is part of the <br> business plan</h3>
        </div>
        
        <div class="col-4 right">
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

  .container {
    padding: 60px 0px;
  }

  .news {
    background-color: $gray_nurse;
  }
    
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
  
  .col-4 {

    filter: brightness(80%);
    position: relative;

    img {
      width: 100%;
      border-radius: 5px;
    
      &:hover {
        filter: blur(2px);
      }
    }
  }

  h3 {
    text-align: center;
    color: $white;
    font-weight: bold;
  }
     
  .left h3, .right h3 {
    position: absolute;
    top: 300px;
    left: 75px;
    color: $white;
  }
  
  .middle h3 {
    position: absolute;
    top: 265px;
    left: 75px;
    color: $white;
  }

  #news {
    @include bg-text2();
  }


</style>