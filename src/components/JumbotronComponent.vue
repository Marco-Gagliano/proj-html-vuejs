<template>

  <div class="jumbotron container-fluid">

    <div class="container">

      <div class="row text-center">
        <div class="col">

          <h6 class="text-uppercase fw-bold">introdution video</h6>
          <h1 class="my-3 fw-bold">Advisory <span id="performance">Performance</span></h1>
          <p>Financial executives need to review their strategies, operating models and capabilities so that their areas can generate sound information for better decision making.</p>

          <div class="jumbo-video">
            <img src="../assets/images/video-1.jpg" alt="Video Jumbotron">
            <a href="#"><i class="fa-solid fa-play sx"></i></a>
            <a href="#"><i class="fa-solid fa-play dx"></i></a>
          </div>

        </div>
      </div>

    </div>

  </div>

</template>


<script>

export default {
  name: 'JumbotronComponent'
}
</script>


<style lang="scss" scoped>

  @import '../assets/style/vars';
  @import '../assets/style/mixins';

  .jumbotron {
    padding: 175px 0
  }

  h6 {
    color: $fountain_blue;
  }

  p {
    margin: 0 300px;
    color: $salt_box;
  }

  img {
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 60%;
    padding: 30px 0;
  }

  .jumbo-video{
    position: relative;
    
    .sx {
      position: absolute;
      color: rgba($color: $blue_lagoon, $alpha: 0.8);
      bottom: 170px;
      left: 618px;
      font-size: 80px;
    }
    
    .dx {
      position: absolute;
      color: rgba($color: $white, $alpha: 0.7);
      bottom: 162px;
      left: 618px;
      font-size: 80px;
    }
  }

  #performance {
    @include bg-text1();
  }


</style>