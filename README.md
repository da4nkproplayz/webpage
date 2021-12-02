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

