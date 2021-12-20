<template>
  <div id="app">
    <!-- Header -->
    <header class="p-3">
      <figure>
        <img src="../images/logo.svg" alt="logo" class="logo">
      </figure>
    </header>

    <!-- Main -->
    <main class="container p-5">
      <div class="row">
        <!-- Figure Mockups -->
        <div class="col col-md-12 col-lg-6">
          <figure>
            <img src="../images/illustration-mockups.svg" alt="illustration-mockup" class="img-fluid">
          </figure>
        </div>
        
        <!-- Text Presentation -->
        <div class="col col-md-12 col-lg-6 text-white text-center text-md-left">
          <h1>Build The Community Your Fans Will Love</h1>
          <p>Huddle re-imagines the way we build communities.
             You have a voice, but so does your audience.
             Create connections with your users as you engage in genuine discussion</p>
             <div class="d-flex justify-content-center">
                <a href="#" class="btn my-btn-light">Register</a>
             </div>
        </div>
      </div>
    </main>

    <!-- Footer Social Menu -->
    <footer>
      <div class="social-menu">
        <div class="circle"><i class="fab fa-facebook-f"></i></div>
        <div class="circle mx-2"><i class="fab fa-twitter"></i></div>
        <div class="circle"><i class="fab fa-instagram"></i></div>

      </div>
    </footer>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;500;700&display=swap');
@import url('https://cdnjs.cloudflare.com/ajax/libs/bootstrap/4.6.1/css/bootstrap.min.css');
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css');

// GENERICS
#app{
  padding: 20px;
}

body{
  background-color: #674bb1;
  background-image: url('../images/bg-desktop.svg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  font-family: 'Open Sans', sans-serif;
}

// HEADER
header{
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.logo{
  width: 200px;
}

// MAIN
.circle{
  border: 1px solid #fff;
  width: 40px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
  border-radius: 50%;
  padding: 6px;
  transition: 0.3s ease;

  &:hover{
    color:#e980e7;
    border-color: #e980e7;
    cursor: pointer;

  }
}

.my-btn-light{
  padding: 10px 60px;
  background-color: #fff;
  border-radius: 60px;
  font-size: 1.1em;
  box-shadow: 1px 2px 5px 6px rgba(0,0,0,0.29);
  transition: 0.3s ease;

  &:hover{
    background-color: #e980e7;
    color:#fff;
  }
}

// FOOTER
.social-menu{
  display: flex;
  justify-content: end;
  align-items: center;
  font-size: 1.4em;

}

// RESPONSIVE
@media only screen and (max-width: 768px) {
  body{
  background-color: #674bb1;
  background-image: url('../images/bg-mobile.svg');
  background-size: cover;
  background-position: center;
  font-family: 'Open Sans', sans-serif;
  background-repeat: no-repeat;
  
  }
  // FOOTER
  .social-menu{
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 1.4em;
  }
}


@media only screen and (max-width: 576px) {
  body{
  background-color: #674bb1;
  background-image: url('../images/bg-mobile.svg');
  background-size: cover;
  background-position: center;
  font-family: 'Open Sans', sans-serif;
  background-repeat: no-repeat;
  
  }
  // FOOTER
  .social-menu{
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 1.4em;
  }
}
</style>
