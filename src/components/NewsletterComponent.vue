<template>
  
  <div class="newsletter container-fluid">
    <div class="container py-5">

      <div class="row">

        <div class="col-6">
          <h6>newsletter</h6>
          <h1 class="my-3">Know First</h1>
          <p>Follow closely and receive content about our company and the news of the current market.</p>
        </div>

        <div class="col-6">
        
          <input type="text" name="" placeholder="Name">
          <input type="text" name="" placeholder="Email">
        
        <br>
        <button>SUBSCRIBE</button>
        </div>

      </div>

    </div>
  </div>

</template>


<script>

export default {
  name: 'NewsletterComponent'
}
</script>


<style lang="scss" scoped>

.newsletter {
  background-color: #111117;

  h6 {
    color: #048383;
    font-weight: bold;
    text-transform: uppercase;
  }

  h1 {
    color: #FFFFFF;
    font-weight: bold;
  }

  p {
    padding-right: 221px;
    color: #BCBDBD;
  }
}

.col-6 {
  
  input {
    margin-bottom: 10px;
    width: 60%;
    padding: 10px;
    border-radius: 5px;
    border: 0;
    background-color: #1D2528;
    color: #BCBDBD;
  }

  button {
    
    background-color: #048383;
    color: #FFFFFF;
    border: none;
    border: 1px solid #048383;
    border-radius: 5px;
    padding: 8px 30px;
  }
}

</style>