<template>
  
  <header>

    <!-- INFO -->
    <div class="info container-fluid">
      <div class="container">
        <div class="row">

          <div class="col-6">
            <i class="fa-solid fa-clock"></i>
            <span> Open Hours: Mon - Sat - 9:00 - 18:00</span>
          </div>

          <div class="col-6">
            <nav>
              <ul>
                <li><a href="#"><i class="fa-solid fa-phone"></i>+1 (305) 1234-5678</a></li>
                <li><a href="#"><i class="fa-solid fa-envelope"></i>hello@examle.com</a></li>
                <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></li>
              </ul>
            </nav>
          </div>

        </div>
      </div>
    </div>
    <!-- /INFO -->
    

    <!-- MENU -->
    <div class="menu-description">
      <div class="menu container-fluid">
        <div class="container">
          <div class="row">

            <div class="col-4 mt-4">
              <p class="text-light">NEXGEN</p>
            </div>

            <div class="col-7 mt-4">

              <ul v-for="(menu, index) in menuList" :key="`menu${index}`">
                <li><a :href="menu.href">{{menu.name}}</a></li>
              </ul>

            </div>

            <div class="col-1 mt-4">
              <a href="#"><i class="fa-regular fa-user"></i></a>
              <button>GET IN TOUCH</button>
            </div>

          </div>
        </div>
      </div>
      <!-- /MENU -->


      <!-- DESCRIPTION -->
      <div class="description text-center">
        <div class="row">
          <div class="col">
            <h1 class="text-light fw-bold">Financial Risk</h1>
            <p>The right outcomes depend on continuos rigor in governance, models, and processes across the finance function</p>
            <button>GET IN TOUCH</button>
            <button>READ MORE</button>  
          </div>
        </div>
      </div>
      <!-- /DESCRIPTION -->

    </div>
    

  </header>

</template>


<script>

export default {
  name: 'HeaderComponent',

  data() {
    return {
      menuList: [
        {
          name: 'HOME',
          href: '#'
        },

        {
          name: 'ABOUT',
          href: '#'
        },

        {
          name: 'SERVICE',
          href: '#'
        },

        {
          name: 'TEAM',
          href: '#'
        },

        {
          name: 'BLOG',
          href: '#'
        },
      ]
    }
  }

}
</script>


<style lang="scss" scoped>

  @import '../assets/style/general';
  

  // GENERAL PRESETS

  .menu-description {
    background-image: url(../assets/images/bg-2.jpg);
    background-size: cover;
    height: 1055px;
  }

  i {
    margin: 0 20px;
    color: #676669
  }

  span {
    color: #676669
  }

  p {
    letter-spacing: 5px;
    font-weight: bold;
  }

  // /GENERAL PRESETS


  // INFO
  .info {
    background-color: #1D2528;
    
  }

  .info a {
    text-decoration: none;
    color: #676669;
  }

  .info ul {
    display: flex;
    flex-direction: row;
  }
  // /INFO
  

  // MENU


  .col-7 {
    display: flex;
    flex-direction: row;
    justify-content: end;
  }

  .col-1 {
    display: flex;
    flex-direction: row;
  }

  .menu a {
    text-decoration: none;
    color: #FFFFFF;
    margin: 0 10px;
  }

  .menu button {
    margin: 0 10px;
    background-color: #52BABB;
    color: #FFFFFF;
    border: none;
    border: 1px solid #000000;
    border-radius: 5px;
    padding: 8px 30px;
  }

  // /MENU


  // DESCRIPTION

  .description {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .description p {
    color: #BCBDBD;
  }

  .description button {
    margin: 0 10px;
    background-color: #52BABB;
    color: #FFFFFF;
    border: none;
    border: 1px solid #000000;
    border-radius: 5px;
    padding: 8px 30px;
  }

  // /DESCRIPTION


  


</style>