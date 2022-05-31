<template>
  
  <div class="team container-fluid">

    <div class="container">

      <h6 class="text-uppercase my-4">we like what we do</h6>
      <div class="row">

        <div class="description-team col-8">

          <h1 class="fw-bold"> <span id="team">Team</span> of Experts</h1>
          <p class="mb-3">Ethics and integrity are the bases on which our professionals build their careers. They are fundamentals that become daily attitudes.</p>

          <div class="row">

            <div class="col-6" v-for="(team, index) in cardTeam" :key="`team${index}`">
              
              <img :src="team.img" :alt="team.name">
              
              <div class="info-team">
                <h3>{{team.name}}</h3>
                <span>{{team.role}}</span>

                <div class="contact-team">
                  <a href="#"><i :class="team.fb"></i></a>
                  <a href="#"><i :class="team.twitter"></i></a>
                  <a href="#"><i :class="team.linkedIn"></i></a>
                </div>

              </div>

            </div>

          </div>

        </div>  

        <div class="col-4">
          <h3>President Speech</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Praesent ut lacinia diam.</p>
          <p>Vivamus efficitur et est quis posuere. Nulla sollicitudin vulputate dui, id pretium tortor congue ue. Integer aliquet justo eu quam volupat ullamcorper.</p>
          <p>Duis ut hendrerit mauris. Phasellus faucibus ut enim vel tincidunt. Nunc venenatis a dui et laoreet</p>
          <span class="py-4">T. Johnson <i class="fa-solid fa-quote-right"></i></span>
        </div>  

      </div>
      
    </div>

  </div>

</template>


<script>

export default {
  name: 'TeamComponent',

  data() {
    return {
      cardTeam: [
        {
          img: require('../assets/images/team-1.jpg'),
          name: 'David Cooper',
          role: 'CTO & CO-FOUNDER',
          fb: 'fa-brands fa-facebook-f',
          twitter: 'fa-brands fa-twitter',
          linkedIn: 'fa-brands fa-linkedin-in',
        },

        {
          img: require('../assets/images/team-3.jpg'),
          name: 'Oliver Jones',
          role: 'CHIEF PROCUREMENT',
          fb: 'fa-brands fa-facebook-f',
          twitter: 'fa-brands fa-twitter',
          linkedIn: 'fa-brands fa-linkedin-in',
        },

        {
          img: require('../assets/images/team-2.jpg'),
          name: 'Emma Lopez',
          role: 'CHIEF MARKETING',
          fb: 'fa-brands fa-facebook-f',
          twitter: 'fa-brands fa-twitter',
          linkedIn: 'fa-brands fa-linkedin-in',
        },

        {
          img: require('../assets/images/team-4.jpg'),
          name: 'T. Johnson',
          role: 'CHIEF PROCUREMENT',
          fb: 'fa-brands fa-facebook-f',
          twitter: 'fa-brands fa-twitter',
          linkedIn: 'fa-brands fa-linkedin-in',
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
    padding: 90px 0;
  }

  h6 {
    color: $fountain_blue;
    font-weight: bold;
  }

  img {
    float: left;
    width: 31%;
    border-radius: 5px;
    margin-right: 20px;
  }

  .col-6 {
    margin: 20px 0;
  }

  .col-4 {
    background-color: $blue_lagoon;
    padding: 35px;
    border-radius: 5px;

    i {
      float: right;
      font-size: 20px;
    }

    h3 {
      color: $white;
      font-weight: bold;
    }

    p {
      color: $silver_sand;
      padding-right: 69px;
      margin: 20px 0;
      font-size: 19px;
    }

    span {
      color: $white;
      font-size: 18px;
      font-weight: bold;
      padding-top: 50px;
    }
  }

  .description-team {

    h1 {
      font-size: 55px;
      color: $woodsmoke;
    }

    #team {
      @include bg-text1();
    }

    p {
    padding-right: 170px;
    color: $salt_box;
    font-size: 19px;
    }

 
  }

  .info-team {

    .contact-team {
      display: flex;
      justify-content: start;
    }

    h3 {
      font-weight: bold;
      color: $woodsmoke;
    }

    span {
      color: $salt_box;
    }

    i {
      color: $blue_lagoon;
      background-color: $gray_nurse;
      font-size: 18px;
      margin: 40px 3px 0px 3px;
      width: 40px;
      height: 40px;
      line-height: 40px;
      text-align: center;
      border-radius: 100px;
    }
  }


</style>