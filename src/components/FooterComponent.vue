<template>
  
  <footer class="container-fluid">
    <div class="contacts container-fluid">
      <div class="container">
        <div class="row">

          <div class="col-3 info">
            <h4><span id="nex">nex</span>gen</h4>          
            <ul>
              
              <li>
                <p>A Functional HTML Template for Corporate & Business.</p>
              </li>
            
              <li>
                <i class="fa-solid fa-phone"></i>
                <span>+1 (305) 1234-5678</span>
              </li>

              <li>
                <i class="fa-solid fa-envelope"></i>
                <span>hello@example.com</span>
              </li>

              <li>
                <i class="fa-solid fa-location-dot"></i>
                <span>Main Avenue, 987</span>
              </li>

              <li>
                <button>GET IN TOUCH</button>           
              </li>
            </ul>

          </div>

          <div class="col-3 contact">

            <ul>
              <li>
                <h3 class="py-3">About</h3>
              </li>
            </ul>

            <ul v-for="(contact, index) in aboutContacts" :key="`aboutContacts${index}`">
              <li>  
                <a :href="contact.href"><i :class="contact.icon"></i>{{contact.name}}</a>
              </li>
            </ul>

          </div>

          <div class="col-3 contact">

            <ul>
              <li>
                <h3 class="py-3">Services</h3>
              </li>
            </ul>

            <ul v-for="(contact, index) in servicesContacts" :key="`servicesContacts${index}`">
              <li>  
                <a :href="contact.href"><i :class="contact.icon"></i>{{contact.name}}</a>
              </li>
            </ul>

          </div>

          <div class="col-3 contact">

            <ul>
              <li>
                <h3 class="py-3">Support</h3>
              </li>
            </ul>

            <ul v-for="(contact, index) in supportContacts" :key="`supportContacts${index}`">
              <li>  
                <a :href="contact.href"><i :class="contact.icon"></i>{{contact.name}}</a>
              </li>
            </ul>

          </div>
          
        </div>
      </div>
    </div>

    <div class="credits container-fluid py-4">
      <div class="container">
        <div class="row d-flex justify-content-between">

          <div class="col-6"> 
            <span>Enjoy the low price. We are Tracking any intention of piracy</span>
          </div>

          <div class="col-6 right">
            <span>@2020 NEXGEN is Proudly Powered by <span id="codings">Codings.</span></span>
          </div>

        </div>
      </div>
    </div>

  </footer>

</template>


<script>

export default {
  name: 'FooterComponent',

  data() {
    return {
      aboutContacts: [
        {
          name: 'The Company',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },
        
        {
          name: 'Institutional',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Social & Events',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Innovation',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Environment',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Technology',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },
      ],

      servicesContacts: [
        {
          name: 'Audit & Assurance',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },
        
        {
          name: 'Financial Advisory',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Analytics M&A',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Middle Marketing',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Legal Consulting',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Regulatory Risk',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },
      ],

      supportContacts: [
        {
          name: 'Responsibility',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },
        
        {
          name: 'Terms of Use',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'About Cookies',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Privacy Policy',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Accessibility',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },

        {
          name: 'Information',
          href: '#',
          icon: 'fa-solid fa-chevron-right',
        },
      ]
    }
  },

}
</script>


<style lang="scss" scoped>

  @import '../assets/style/vars';
  @import '../assets/style/mixins';

  footer {
    padding: 0;
  }

  .contacts {
    background-image: url(../assets/images/bg-7.jpg);
    background-position: center;
    color: $silver_sand;
    padding: 125px 0px;

    ul {
      margin-bottom: 0px;
    }

    i {
      padding-right: 10px;
    }

  }

  .info {

    #nex {
      @include bg-text4()
    }

    h4 {
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 5px;
      margin-bottom: 35px;
    }

    p {
      padding-right: 70px;
    }

    ul {
      padding: 0;
    }

    li {
      padding-bottom: 22px;
      font-size: 18px;
    }

    button {
      @include button_type2();
    }

  }

  .contact {
    background-color: rgba($color: $shark, $alpha: 0.4);
    border-radius: 10px;
    margin-left: 30px;
    padding: 30px 0px;
    width: 22.7%;

    h3 {
      font-weight: bold;
      color: $gray_nurse;
    }

    ul {
      margin: 10px;
      font-size: 17px;

      a {
        color: $silver_sand;
      }
    }
  }

  .credits {
    color: $silver_sand;
    background-color: $black;

    .right {
      display: flex;
      justify-content: end;
    }

    #codings {
      color: $blue_lagoon
    }
  }

</style>