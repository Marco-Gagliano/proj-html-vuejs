<template>
  
  <header>

    <!-- INFO -->
    <div class="info container-fluid">
      <div class="container">
        <div class="row py-3">

          <div class="col-6 opening-hours">
            <i class="fa-solid fa-clock"></i>
            <span> Open Hours: Mon - Sat - 9:00 - 18:00</span>
          </div>

          <div class="col-6 contacts">
            <nav>
              <ul>
                <li><a href="#"><i class="fa-solid fa-phone"></i>+1 (305) 1234-5678</a></li>
                <li><a href="#"><i class="fa-solid fa-envelope"></i>hello@example.com</a></li>
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

            <div class="col-2 mt-4">
              <h5><span id="nex">NEX</span>GEN</h5>
            </div>

            <div class="col-7 mt-4">

              <ul v-for="(menu, index) in menuList" :key="`menu${index}`">
                <li><a :href="menu.href">{{menu.name}}</a></li>
              </ul>
              <ul>
                <li><a href="#"><i class="fa-regular fa-user"></i></a></li>
              </ul>
            </div>


            <div class="col-2 mt-4">
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
            <h1 class="my-4">Financial Risk</h1>
            <p>The right outcomes depend on continuos rigor in governance, models, and <br>processes across the finance function</p>
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
  @import '../assets/style/vars';
  @import '../assets/style/mixins';
  

  // GENERAL PRESETS

  .menu-description {
    //background-image: url(../assets/images/bg-2.jpg);
    background: linear-gradient(
            rgba(0, 0, 0, 0.3), 
            rgba(0, 0, 0, 0.3)
    ),
    url(../assets/images/bg-2.jpg);
    background-size: cover;
    height: 1055px;
  }

  .contacts {
    display: flex;    
    justify-content: end;

    i {
      margin-left: 20px;
      margin-right: 10px;
      color: $salt_box;
    }

    p {
      letter-spacing: 5px;
      font-weight: bold;
    }
  }

  span {
    color: $salt_box;
  }

  h5 {
    color: $gray_nurse;
    font-weight: bold;
    letter-spacing: 5px;
    margin-left: 10px;

    #nex {
      @include bg-text4()
    }
  }

  // /GENERAL PRESETS


  // INFO
  .info {
    background-color: $shark;

    .col-6 {
      display: flex;
      align-items: center;
    }
  }

  .opening-hours i {
    margin-right: 8px ;
    color: $salt_box;
  }
  .info a {
    text-decoration: none;
    color: $salt_box;
  }

  .info ul {
    display: flex;
    flex-direction: row;
    margin: 0;
  }
  // /INFO
  

  // MENU

  .col-7 {
    display: flex;
    flex-direction: row;
    justify-content: end;
  }
  
  .col-2 {
    display: flex;
    flex-direction: row;
    justify-content: end;
  }

  .menu a {
    text-decoration: none;
    color: $white;
    margin: 0 10px;
  }

  button {
    @include button_type1();
  }

  // /MENU


  // DESCRIPTION

  .description {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 270px;

    h1 {
      font-size: 70px;
      font-weight: bold;
      color: $white;
    }

    p {
      color: #BCBDBD;
      font-size: 19px;
      
    }

    button {
      @include button_type2();
      margin: 0 10px;
    }

  }

  // /DESCRIPTION
 
</style>