<template>
  
  <header class="container-fluid">

    <div class="container">
      <div class="contact-info">
        <div class="row">
          <div class="col-6">orario lavorativo</div>
          <div class="col-6">
            <ul>
              <li>telefono </li>
              <li>email </li>
              <li>facebook </li>
              <li>twitter </li>
              <li>linkedin </li>
            </ul>
          </div>
        </div>
      </div>
    

      <div class="menu">
        <div class="row">
          <div class="col-6">nexgen</div>
          <div class="col-6">
            <ul>
              <li><a href="#">HOME</a></li>
              <li><a href="#">ABOUT</a></li>
              <li><a href="#">SERVICE</a></li>
              <li><a href="#">TEAM</a></li>
              <li><a href="#">BLOG</a></li>
              <li><a href="#">ICONA PROFILO</a></li>
              <button>GET IN TOUCH</button>
            </ul>
          </div>
        </div>
      </div>

      <div class="description text-center">
        <div class="row">
          <div class="col">
            <h1>financial risk</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos impedit dolores quidem?</p>
            <button>GET IN TOUCH</button>
            <button>READ MORE</button>  
          </div>
        </div>
      </div>

    </div>

  </header>

</template>


<script>

export default {
  name: 'HeaderComponent'

}
</script>


<style lang="scss" scoped>

  header {
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