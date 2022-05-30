<template>
  
  <footer class="container-fluid">
    <div class="contacts container-fluid py-5">
      <div class="container py-5">
        <div class="row">

          <div class="col-3 info">
            <h4>nexgen</h4>          
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
                <span>hello@spanle.com</span>
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
                <h3>About</h3>
              </li>
            </ul>

            <ul v-for="(contact, index) in aboutContacts" :key="`aboutContacts${index}`">
              <li>  
                <a :href="contact.href"><i :class="contact.icon"></i>
                {{contact.name}}</a>
              </li>
            </ul>

          </div>

          <div class="col-3 contact">

            <ul>
              <li>
                <h3>Services</h3>
              </li>
            </ul>

            <ul v-for="(contact, index) in servicesContacts" :key="`servicesContacts${index}`">
              <li>  
                <a :href="contact.href"><i :class="contact.icon"></i>
                {{contact.name}}</a>
              </li>
            </ul>

          </div>

          <div class="col-3 contact">

            <ul>
              <li>
                <h3>Support</h3>
              </li>
            </ul>

            <ul v-for="(contact, index) in supportContacts" :key="`supportContacts${index}`">
              <li>  
                <a :href="contact.href"><i :class="contact.icon"></i>
                {{contact.name}}</a>
              </li>
            </ul>

          </div>
          
        </div>

      </div>
    </div>

    <div class="credits container-fluid">
      <div class="container">
        <div class="row d-flex align-items-center">

          <div class="col-6"> 
            <p>Enjoy the low price. We are Tracking any intention of piracy</p>
          </div>

          <div class="col-6 d-flex justify-content-end align-items-center">
            <p>@2020 NEXGEN is Proudly Powered by Codings.</p>
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

    ul {
      margin-bottom: 0px;
    }
  }

  .info {
    ul {
      padding: 0;
    }

  }


  h4 {
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 5px;
  }

  h3 {
    font-weight: bold;
    color: $gray_nurse;
  }

  p {
    padding-right: 80px;
  }


  i {
    padding-right: 10px;
  }
  
  button {
    @include button_type2();
  }

  .contact {
    background-color: rgba($color: $shark, $alpha: 0.4);
    border-radius: 10px;
    margin-right: 30px;
    width: calc(100% / 5);

    ul {
      margin: 10px;
      font-size: 20px;

      a {
        color: $silver_sand;
      }
    }
  }
  


  .credits {
    color: $silver_sand;
    background-color: $woodsmoke;
  }

    .col-6 {
      float: right;
    }
</style>