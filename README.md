<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Scroll Website</title>
    <link rel="stylesheet" href="styles.css" />
    <link
      rel="stylesheet"
      href="https://use.fontawesome.com/releases/v5.14.0/css/all.css"
      integrity="sha384-HzLeBuhoNPvSl5KYnjx0BT+WB0QEEqLprO+NBkkk5gbc67FTaL7XIGa2w1L0Xbgc"
      crossorigin="anonymous"
    />
  </head>
  <body>
    <!-- Navbar Section -->
    <nav class="navbar">
      <div class="navbar__container">
        <a href="#home" id="navbar__logo">COLOR</a>
        <div class="navbar__toggle" id="mobile-menu">
          <span class="bar"></span> <span class="bar"></span>
          <span class="bar"></span>
        </div>
        <ul class="navbar__menu">
          <li class="navbar__item">
            <a href="#home" class="navbar__links" id="home-page">Home</a>
          </li>
          <li class="navbar__item">
            <a href="#about" class="navbar__links" id="about-page">About</a>
          </li>
          <li class="navbar__item">
            <a href="#services" class="navbar__links" id="services-page"
              >Services</a
            >
          </li>
          <li class="navbar__btn">
            <a href="#sign-up" class="button" id="signup">Sign Up</a>
          </li>
        </ul>
      </div>
    </nav>

    <!-- Hero Section -->
    <div class="hero" id="home">
      <div class="hero__container">
        <h1 class="hero__heading">Choose your <span>colors</span></h1>
        <p class="hero__description">Unlimited Possibilities</p>
        <button class="main__btn"><a href="#">Explore</a></button>
      </div>
    </div>

    <!-- About Section -->
    <div class="main" id="about">
      <div class="main__container">
        <div class="main__img--container">
          <div class="main__img--card"><i class="fas fa-layer-group"></i></div>
        </div>
        <div class="main__content">
          <h1>What do i do?</h1>
          <h2>i am learning computer programing</h2>
          <p>I am currently learning Java, JavaScript, Python, arduino, and web development</p>
        </div>
      </div>
    </div>

    <!-- Services Section -->
    <div class="services" id="services">
      <h1>Our Services</h1>
      <div class="services__wrapper">
        <div class="services__card">
          <h2>Custom Colorways</h2>
          <p>AI Powered technology</p>
          <div class="services__btn"><button>Get Started</button></div>
        </div>
        <div class="services__card">
          <h2>Are you Ready?</h2>
          <p>Take the lepa</p>
          <div class="services__btn"><button>Get Started</button></div>
        </div>
        <div class="services__card">
          <h2>Full Gradients</h2>
          <p>100 Combinations</p>
          <div class="services__btn"><button>Get Started</button></div>
        </div>
        <div class="services__card">
          <h2>Infinite Choices</h2>
          <p>1000's of colors</p>
          <div class="services__btn"><button>Get Started</button></div>
        </div>
      </div>
    </div>

   
        </div>
      </section>
    </div>

    <script src="app.js"></script>
  </body>
</html>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: "Kumbh Sans", sans-serif;
    scroll-behavior: smooth;
  }

  .navbar {
    background: #131313;
    height: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 1.2rem;
    position: sticky;
    top: 0;
    z-index: 999;
  }

  .navbar__container {
    display: flex;
    justify-content: space-between;
    height: 80px;
    z-index: 1;
    width: 100%;
    max-width: 1300px;
    margin: 0 auto;
    padding: 0 50px;
  }

  #navbar__logo {
    background-color: #ff8177;
    background-image: linear-gradient(to top, #ff0844 0%, #ffb199 100%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
    display: flex;
    align-items: center;
    cursor: pointer;
    text-decoration: none;
    font-size: 2rem;
  }

  .navbar__menu {
    display: flex;
    align-items: center;
    list-style: none;
  }

  .navbar__item {
    height: 80px;
  }

  .navbar__links {
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 125px;
    text-decoration: none;
    height: 100%;
    transition: all 0.3s ease;
  }

  .navbar__btn {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 1rem;
    width: 100%;
  }

  .button {
    display: flex;
    justify-content: center;
    align-items: center;
    text-decoration: none;
    padding: 10px 20px;
    height: 100%;
    width: 100%;
    border: none;
    outline: none;
    border-radius: 4px;
    background: #833ab4;
    background: -webkit-linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
    background: linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
    color: #fff;
    transition: all 0.3s ease;
  }

  .navbar__links:hover {
    color: #9518fc;
    transition: all 0.3s ease;
  }

  @media screen and (max-width: 960px) {
    .navbar__container {
      display: flex;
      justify-content: space-between;
      height: 80px;
      z-index: 1;
      width: 100%;
      max-width: 1300px;
      padding: 0;
    }

    .navbar__menu {
      display: grid;
      grid-template-columns: auto;
      margin: 0;
      width: 100%;
      position: absolute;
      top: -1000px;
      opacity: 1;
      transition: all 0.5s ease;
      z-index: -1;
    }

    .navbar__menu.active {
      background: #131313;
      top: 100%;
      opacity: 1;
      transition: all 0.5s ease;
      z-index: 99;
      height: 60vh;
      font-size: 1.6rem;
    }

    #navbar__logo {
      padding-left: 25px;
    }

    .navbar__toggle .bar {
      width: 25px;
      height: 3px;
      margin: 5px auto;
      transition: all 0.3s ease-in-out;
      background: #fff;
    }

    .navbar__item {
      width: 100%;
    }

    .navbar__links {
      text-align: center;
      padding: 2rem;
      width: 100%;
      display: table;
    }

    .navbar__btn {
      padding-bottom: 2rem;
    }

    .button {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 80%;
      height: 80px;
      margin: 0;
    }

    #mobile-menu {
      position: absolute;
      top: 20%;
      right: 5%;
      transform: translate(5%, 20%);
    }

    .navbar__toggle .bar {
      display: block;
      cursor: pointer;
    }

    #mobile-menu.is-active .bar:nth-child(2) {
      opacity: 0;
    }

    #mobile-menu.is-active .bar:nth-child(1) {
      transform: translateY(8px) rotate(45deg);
    }

    #mobile-menu.is-active .bar:nth-child(3) {
      transform: translateY(-8px) rotate(-45deg);
    }
  }

  /* Hero Section */
  .hero {
    background: #000000;
    background: linear-gradient(to right, #161616, #000000);
    padding: 200px 0;
  }

  .hero__container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    height: 90%;
    text-align: center;
    padding: 30px;
  }

  .hero__heading {
    font-size: 100px;
    margin-bottom: 24px;
    color: #fff;
  }

  .hero__heading span {
    background: #ee0979; 
    background: -webkit-linear-gradient(
      to right,
      #ff6a00,
      #ee0979
    ); 
    background: linear-gradient(
      to right,
      #ff6a00,
      #ee0979
    ); 
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -mo-text-fill-color: transparent;
  }

  .hero__description {
    font-size: 60px;
    background: #da22ff; 
    background: -webkit-linear-gradient(
      to right,
      #9114ff,
      #da22ff
    ); 
    background: linear-gradient(
      to right,
      #8f0eff,
      #da22ff
    ); 
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
  }

  .highlight {
    border-bottom: 4px solid rgb(132, 0, 255);
  }

  @media screen and (max-width: 768px) {
    .hero__heading {
      font-size: 60px;
    }

    .hero__description {
      font-size: 40px;
    }
  }

  /* About Section */
  .main {
    background-color: #131313;
    padding: 10rem 0;
  }

  .main__container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    justify-content: center;
    margin: 0 auto;
    height: 90%;
    z-index: 1;
    width: 100%;
    max-width: 1300px;
    padding: 0 50px;
  }

  .main__content {
    color: #fff;
    width: 100%;
  }

  .main__content h1 {
    font-size: 2rem;
    background-color: #fe3b6f;
    background-image: linear-gradient(to top, #ff087b 0%, #ed1a52 100%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
    text-transform: uppercase;
    margin-bottom: 32px;
  }

  .main__content h2 {
    font-size: 4rem;
    background: #ff8177; 
    background: -webkit-linear-gradient(
      to right,
      #9114ff,
      #da22ff
    ); 
    background: linear-gradient(
      to right,
      #8f0eff,
      #da22ff
    );
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
  }

  .main__content p {
    margin-top: 1rem;
    font-size: 2rem;
    font-weight: 700;
  }

  .main__btn {
    font-size: 1.8rem;
    background: #833ab4;
    background: -webkit-linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
    background: linear-gradient(to right, #fcb045, #fd1d1d, #833ab4);
    padding: 20px 60px;
    border: none;
    border-radius: 4px;
    margin-top: 2rem;
    cursor: pointer;
    position: relative;
    transition: all 0.35s;
    outline: none;
  }

  .main__btn a {
    position: relative;
    z-index: 2;
    color: #fff;
    text-decoration: none;
  }

  .main__btn:after {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: #ff1ead;
    transition: all 0.35s;
    border-radius: 4px;
  }

  .main__btn:hover {
    color: #fff;
  }

  .main__btn:hover:after {
    width: 100%;
  }

  .main__img--container {
    text-align: center;
  }

  .main__img--card {
    margin: 10px;
    height: 500px;
    width: 500px;
    border-radius: 4px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: #fff;
    background-image: linear-gradient(to right, #00dbde 0%, #fc00ff 100%);
  }

  .fa-layer-group,
  .fa-users {
    font-size: 14rem;
  }

  #card-2 {
    background: #ff512f;
    background: -webkit-linear-gradient(to right, #dd2476, #ff512f);
    background: linear-gradient(to right, #dd2476, #ff512f);
  }

  /* Mobile Responsive */
  /*this is basically how the webpage would look on a phone*/
  @media screen and (max-width: 1100px) {
    .main__container {
      display: grid;
      grid-template-columns: 1fr;
      align-items: center;
      justify-content: center;
      width: 100%;
      margin: 0 auto;
      height: 90%;
    }

    .main__img--container {
      display: flex;
      justify-content: center;
    }

    .main__img--card {
      height: 425px;
      width: 425px;
    }

    .main__content {
      text-align: center;
      margin-bottom: 4rem;
    }

    .main__content h1 {
      font-size: 2.5rem;
      margin-top: 2rem;
    }

    .main__content h2 {
      font-size: 3rem;
    }

    .main__content p {
      margin-top: 1rem;
      font-size: 1.5rem;
    }
  }

  @media screen and (max-width: 480px) {
    .main__img--card {
      width: 250px;
      height: 250px;
    }

    .fa-users,
    .fa-layer-group {
      font-size: 4rem;
    }

    .main__content h1 {
      font-size: 2rem;
      margin-top: 3rem;
    }
    .main__content h2 {
      font-size: 2rem;
    }

    .main__content p {
      margin-top: 2rem;
    }

    .main__btn {
      padding: 12px 36px;
      margin: 2.5rem 0;
    }
  }

  /*the services section and Its content like the boxes*/
  .services {
    background: #131313;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100%;
    padding: 10rem 0;
  }

  .services h1 {
    background-color: #ff8177;
    background-image: linear-gradient(to right, #ff0844 0%, #f7673c 100%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
    margin-bottom: 5rem;
    font-size: 2.5rem;
  }

  .services__wrapper {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-rows: 1fr;
  }

  .services__card {
    margin: 10px;
    height: 425px;
    width: 300px;
    border-radius: 4px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: #fff;
    background-image: linear-gradient(to right, #00dbde 0%, #fc00ff 100%);
    transition: 0.3s ease-in;
    text-align: center;
    
  }
  



</style>
