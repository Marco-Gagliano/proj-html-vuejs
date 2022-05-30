<template>

  <div class="jumbotron container-fluid">

    <div class="container">

      <div class="row text-center">
        <div class="col">
          <span class="text-uppercase fw-bold">introdution video</span>
          <h1 class="my-3 fw-bold">Advisory Performance</h1>
          <p>Financial executives need to review their strategies, operating models and capabilities so that their areas can generate sound information for better decision making.</p>
          <img src="../assets/images/video-1.jpg" alt="Video Jumbotron">
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
    padding: 100px 0
  }

  span {
    color: $blue_lagoon;
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

</style>