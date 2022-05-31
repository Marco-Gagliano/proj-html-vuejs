<template>

  <div class="service container-fluid">
    <div class="container">

      <div class="info-service">

        <h6 class="pt-5">OUR BUSINESS AREAS</h6>
        <h1>Excellent in <span id="services">Services</span> </h1>

        <div class="row my-4">

          <div class="col-9">
            <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.</p>
          </div>

          <div class="col-3">
            <button>SEE ALL</button>
          </div>

        </div>
        
      </div>

      <div class="description-service">
        <div class="row">

          <div class="col-3" v-for="(service, index) in serviceList" :key="`service${index}`">
            <a :href="service.href">
              <i :class="service.iconLink"></i>
              <i :class="service.iconList"></i>
              <h5>{{service.name}}</h5>
              <p>{{service.text}}</p>
            </a>
          </div>

        </div>
      </div>

    </div>
  </div>

</template>


<script>

export default {
  name: 'BusinessComponent',

  data() {
    return {
      serviceList: [
        {
          name: 'Audit & Assurance',
          text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',
          href: '#',
          iconList: 'fa-solid fa-network-wired',
          iconLink: 'fa-solid fa-arrow-right',
        },

        {
          name: 'Financial Advisory',
          text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',
          href: '#',
          iconList: 'fa-solid fa-briefcase',
          iconLink: 'fa-solid fa-arrow-right',
        },

        {
          name: 'Analytics and M&A',
          text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',
          href: '#',
          iconList: 'fa-solid fa-chart-simple',
          iconLink: 'fa-solid fa-arrow-right',
        },

        {
          name: 'Middle Marketing',
          text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',
          href: '#',
          iconList: 'fa-solid fa-plane-up',
          iconLink: 'fa-solid fa-arrow-right',
        },

        {
          name: 'Legal Consulting',
          text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',
          href: '#',
          iconList: 'fa-solid fa-globe',
          iconLink: 'fa-solid fa-arrow-right',
        },

        {
          name: 'Regulatory Risk',
          text: 'Lorem ipsum dolor sit amet consectetur, adipisicing elit.',
          href: '#',
          iconList: 'fa-solid fa-inbox',
          iconLink: 'fa-solid fa-arrow-right',
        },
      ]
    }
  }

}
</script>


<style lang="scss" scoped>

  @import '../assets/style/vars';
  @import '../assets/style/mixins';

  .container {
    padding: 200px 0px;
  }

  .service {
    background-color: $woodsmoke;
  }

  h1, h5, h6 {
    font-weight: bold;
  }

  h5 {
    padding: 10px 0;
  }

  h6 {
    color: $blue_lagoon
  }

  h1 {
    color: $white
  }

  p {
    color: $silver_sand;
    padding-right: 33px;
    font-size: 20px;
  }

  a {
    text-decoration: none;
  }

  #services {
    @include bg-text3();
  }

  .info-service h1 {
    font-size: 52px;
  }

  .col-3 button {
    @include button_type2();
    float: right;
  }  

  .description-service h5 {
    color: $white;
  }

  .description-service .col-3 {
    background-color: $shark;
    margin: 15px;
    padding: 30px 50px;
    border-radius: 7px;
    width: 31%;

    &:hover {
      .fa-arrow-right {
        background-color: $blue_lagoon;
        color: $white;
        width: 30px;
        height: 30px;
        line-height: 30px;
        border-radius: 50px;
        text-align: center;
      }

      i {
        color: $white;
      }

      p {
        color: $white;
      }
    }
  }

  .description-service {

    i {
      color: $blue_lagoon;
      font-size: 40px;
    }

    .fa-arrow-right {
      float: right;
      font-size: 24px;
      color: $surfie_green;
      transition: ease-in .1s;
      text-align: center;
    }
  }


</style>