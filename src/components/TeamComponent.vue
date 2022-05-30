<template>
  
  <div class="team container-fluid my-5">

    <div class="container">

      <h6 class="text-uppercase mt-5">we like what we do</h6>
      <div class="row">

        <div class="description-team col-8">
          <h1 class="fw-bold">Team of Experts</h1>
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

            
            <!-- <div class="col-6">
              
              <img src="../assets/images/team-2.jpg" alt="Emma Lopez Image">
              
              <div class="info-team">
                <h3>Emma Lopez</h3>
                <span>CHIEF MARKETING</span>

                <div class="contact-team">
                  <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                  <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
                </div>

              </div>
            </div>
            
            <div class="col-6">
              
              <img src="../assets/images/team-4.jpg" alt="T. Johnson Image">
              
              <div class="info-team">
                <h3>T. Johnson</h3>  
                <span>CEO & PRESIDENT</span>

                <div class="contact-team">
                  <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                  <a href="#"><i class="fa-brands fa-twitter"></i></a>
                  <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
                </div>

              </div>
            </div> -->

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

h6 {
  color: #52BABB;
  font-weight: bold;
}

.col-6 img {
  float: left;
  width: 31%;
  border-radius: 5px;
  margin-right: 20px;
}

.col-6 {
  margin: 20px 0;
  
}

.col-4 {
  background-color: #048383;
  padding: 35px;
  border-radius: 5px;

  i {
    float: right;
    font-size: 20px;
  }

  h3 {
    color: #FFFFFF;
    font-weight: bold;
  }

  p {
    color: #BCBDBD;
    padding-right: 69px;
    margin: 20px 0;
    font-size: 19px;
  }

  span {
    color: #FFFFFF;
    font-size: 18px;
    font-weight: bold;
    padding-top: 50px;
    
  }
}

.description-team h1 {
  font-size: 65px;
}
.description-team p {
  padding-right: 150px;
  color: #676669;
  font-size: 19px;
}

.contact-team  {
  display: flex;
  justify-content: start;
}

.info-team {

  h3 {
    font-weight: bold;
  }

  span {
    color: #676669
  }

  i {
    color: #048383;
    background-color: #E7EEE9;
    font-size: 18px;
    margin: 28px 16px;
    padding: 10px;
    border-radius: 100px;
  }
}

  

</style>