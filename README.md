<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>ADI WEB STUDIO — Modern Websites</title>
<meta name="description" content="ADI WEB STUDIO creates clean, modern websites for small businesses.">

<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}

html{
  scroll-behavior:smooth;
}

body{
  font-family:Arial,Helvetica,sans-serif;
  background:#fff;
  color:#15171a;
  line-height:1.6;
}

a{
  color:inherit;
  text-decoration:none;
}

button{
  font:inherit;
}

.container{
  width:min(1120px,92%);
  margin:auto;
}

/* HEADER */

header{
  position:sticky;
  top:0;
  z-index:1000;
  background:rgba(255,255,255,.96);
  border-bottom:1px solid #e8e8e8;
}

.nav{
  min-height:70px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:20px;
}

.logo{
  font-size:19px;
  font-weight:800;
  letter-spacing:-.5px;
}

.logo span{
  color:#2563eb;
}

.nav-links{
  display:flex;
  gap:28px;
  font-size:14px;
  color:#555;
}

.nav-links a:hover{
  color:#2563eb;
}

/* BUTTONS */

.btn{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  padding:12px 18px;
  border:1px solid #15171a;
  border-radius:8px;
  cursor:pointer;
  font-weight:700;
  font-size:14px;
  background:#15171a;
  color:#fff;
  transition:.2s;
}

.btn:hover{
  transform:translateY(-2px);
}

.btn.secondary{
  background:#fff;
  color:#15171a;
  border-color:#d8d8d8;
}

/* HERO */

.hero{
  padding:110px 0 90px;
  border-bottom:1px solid #eee;
}

.hero-grid{
  display:grid;
  grid-template-columns:1.3fr .7fr;
  gap:70px;
  align-items:center;
}

.eyebrow{
  color:#2563eb;
  font-size:13px;
  font-weight:800;
  letter-spacing:1.5px;
  text-transform:uppercase;
  margin-bottom:18px;
}

h1{
  font-size:clamp(46px,7vw,76px);
  line-height:1.02;
  letter-spacing:-4px;
  margin-bottom:25px;
}

.hero p{
  max-width:600px;
  color:#666;
  font-size:18px;
  margin-bottom:30px;
}

.hero-buttons{
  display:flex;
  gap:12px;
  flex-wrap:wrap;
}

.hero-card{
  border:1px solid #ddd;
  padding:28px;
  background:#fafafa;
}

.hero-card strong{
  display:block;
  font-size:40px;
  margin-bottom:5px;
}

.hero-card p{
  font-size:14px;
  margin:0;
}

/* SECTIONS */

section{
  padding:90px 0;
}

.section-head{
  display:flex;
  justify-content:space-between;
  align-items:end;
  gap:30px;
  margin-bottom:35px;
}

.section-head h2{
  font-size:38px;
  letter-spacing:-1.5px;
}

.section-head p{
  color:#777;
  max-width:480px;
}

/* PROJECTS */

.projects{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
}

.project{
  border:1px solid #ddd;
  background:#fff;
  cursor:pointer;
  transition:.25s;
}

.project:hover{
  transform:translateY(-5px);
  border-color:#aaa;
}

.project-preview{
  height:230px;
  padding:22px;
  display:flex;
  align-items:center;
  justify-content:center;
}

.nexora-preview{
  background:#f5f7fa;
}

.cafe-preview{
  background:#f4f0e9;
}

.auto-preview{
  background:#eef1f4;
}

.preview-window{
  width:90%;
  height:75%;
  background:#fff;
  border:1px solid #ddd;
  box-shadow:0 12px 30px rgba(0,0,0,.08);
  padding:16px;
}

.preview-line{
  height:7px;
  background:#ddd;
  margin-bottom:9px;
  width:70%;
}

.preview-line.small{
  width:40%;
}

.preview-box{
  height:65px;
  background:#f1f1f1;
  margin-top:18px;
}

.project-info{
  padding:22px;
  border-top:1px solid #eee;
}

.project-info h3{
  margin-bottom:6px;
}

.project-info p{
  color:#777;
  font-size:14px;
}

/* SERVICES */

.services{
  background:#f7f7f7;
}

.service-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
}

.service{
  background:#fff;
  border:1px solid #ddd;
  padding:28px;
}

.service-number{
  color:#2563eb;
  font-weight:800;
  margin-bottom:30px;
}

.service h3{
  margin-bottom:10px;
}

.service p{
  color:#777;
  font-size:14px;
}

/* ABOUT */

.about-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:70px;
}

.about-grid h2{
  font-size:42px;
  line-height:1.1;
  letter-spacing:-1.5px;
}

.about-grid p{
  color:#666;
  margin-bottom:20px;
}

.facts{
  border-top:1px solid #ddd;
}

.fact{
  display:flex;
  justify-content:space-between;
  padding:16px 0;
  border-bottom:1px solid #ddd;
}

.fact span:last-child{
  font-weight:700;
}

/* CONTACT */

.contact{
  background:#15171a;
  color:#fff;
}

.contact-box{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:60px;
  align-items:center;
}

.contact h2{
  font-size:48px;
  line-height:1.05;
  letter-spacing:-2px;
}

.contact p{
  color:#aaa;
  margin-top:18px;
}

.contact-card{
  background:#fff;
  color:#15171a;
  padding:30px;
}

.contact-card p{
  color:#777;
  margin-bottom:15px;
}

.email{
  color:#2563eb;
  font-weight:700;
  word-break:break-word;
}

/* FOOTER */

footer{
  background:#15171a;
  border-top:1px solid #333;
  color:#888;
  padding:25px 0;
  font-size:13px;
}

/* DEMO PAGES */

.page{
  display:none;
}

.page.active{
  display:block;
}

.demo{
  min-height:100vh;
  background:#fff;
}

.demo-top{
  padding:25px 0;
  border-bottom:1px solid #eee;
}

.back{
  background:#fff;
  border:1px solid #ddd;
  padding:9px 14px;
  border-radius:7px;
  cursor:pointer;
}

.demo-nav{
  padding:20px 0;
  border-bottom:1px solid #eee;
}

.demo-nav-inner{
  display:flex;
  justify-content:space-between;
  align-items:center;
}

.demo-logo{
  font-weight:800;
  font-size:20px;
}

.demo-links{
  display:flex;
  gap:20px;
  font-size:14px;
  color:#666;
}

.demo-hero{
  padding:100px 0;
  background:#f7f8fa;
}

.demo-hero h1{
  max-width:800px;
  font-size:clamp(44px,7vw,72px);
}

.demo-hero p{
  max-width:600px;
  color:#666;
  font-size:18px;
  margin:25px 0;
}

.demo-section{
  padding:80px 0;
}

.demo-section h2{
  font-size:38px;
  margin-bottom:35px;
}

.demo-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
}

.demo-card{
  border:1px solid #ddd;
  padding:28px;
}

.demo-card h3{
  margin-bottom:10px;
}

.demo-card p{
  color:#777;
  font-size:14px;
}

.demo-footer{
  background:#15171a;
  color:#aaa;
  padding:35px 0;
}

/* CAFE */

.cafe .demo-hero{
  background:#f5f0e7;
}

.cafe .demo-hero h1{
  font-family:Georgia,serif;
  letter-spacing:-2px;
}

.menu{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:18px;
}

.menu-item{
  display:flex;
  justify-content:space-between;
  gap:20px;
  padding:22px 0;
  border-bottom:1px solid #ddd;
}

.menu-item p{
  color:#777;
  font-size:14px;
}

.price{
  font-weight:800;
}

/* AUTOCARE */

.autocare .demo-hero{
  background:#111;
  color:#fff;
}

.autocare .demo-hero p{
  color:#aaa;
}

.auto-box{
  border:1px solid #ddd;
  padding:30px;
}

.auto-price{
  font-size:28px;
  font-weight:800;
  margin:10px 0;
}

/* MOBILE */

@media(max-width:800px){

  .nav-links{
    display:none;
  }

  .hero{
    padding:75px 0;
  }

  .hero-grid,
  .about-grid,
  .contact-box{
    grid-template-columns:1fr;
  }

  h1{
    letter-spacing:-2.5px;
  }

  .projects,
  .service-grid,
  .demo-grid{
    grid-template-columns:1fr;
  }

  .section-head{
    display:block;
  }

  .section-head h2{
    margin-bottom:12px;
  }

  .contact h2{
    font-size:40px;
  }

  .menu{
    grid-template-columns:1fr;
  }

  .demo-links{
    display:none;
  }
}
</style>
</head>

<body>

<!-- ================= HOME ================= -->

<div id="home" class="page active">

<header>
  <div class="container nav">

    <a href="#" class="logo" onclick="showPage('home')">
      ADI <span>WEB STUDIO</span>
    </a>

    <nav class="nav-links">
      <a href="#work">Work</a>
      <a href="#services">Services</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>

    <a class="btn" href="#contact">Let's Talk</a>

  </div>
</header>


<main>

<section class="hero">

  <div class="container hero-grid">

    <div>

      <div class="eyebrow">
        Web Design Studio
      </div>

      <h1>
        Modern websites for small businesses.
      </h1>

      <p>
        Clean, responsive websites designed to help small businesses
        look professional and make a strong first impression online.
      </p>

      <div class="hero-buttons">
        <a href="#work" class="btn">View My Work</a>
        <a href="#contact" class="btn secondary">Contact Me</a>
      </div>

    </div>

    <div class="hero-card">
      <strong>03</strong>
      <p>
        Website concepts created for different types of small businesses.
      </p>
    </div>

  </div>

</section>


<section id="work">

  <div class="container">

    <div class="section-head">

      <div>
        <div class="eyebrow">Selected Work</div>
        <h2>Projects</h2>
      </div>

      <p>
        Explore the demo websites below. Each project is designed
        as a realistic business website concept.
      </p>

    </div>


    <div class="projects">


      <!-- NEXORA -->

      <article class="project" onclick="showPage('nexora')">

        <div class="project-preview nexora-preview">

          <div class="preview-window">

            <div class="preview-line small"></div>
            <div class="preview-line"></div>
            <div class="preview-box"></div>

          </div>

        </div>

        <div class="project-info">

          <h3>NEXORA</h3>

          <p>
            Business solutions website concept.
          </p>

        </div>

      </article>


      <!-- CAFE -->

      <article class="project" onclick="showPage('cafe')">

        <div class="project-preview cafe-preview">

          <div class="preview-window">

            <div class="preview-line small"></div>
            <div class="preview-line"></div>
            <div class="preview-box"></div>

          </div>

        </div>

        <div class="project-info">

          <h3>Corner & Co.</h3>

          <p>
            Modern café website concept.
          </p>

        </div>

      </article>


      <!-- AUTOCARE -->

      <article class="project" onclick="showPage('autocare')">

        <div class="project-preview auto-preview">

          <div class="preview-window">

            <div class="preview-line small"></div>
            <div class="preview-line"></div>
            <div class="preview-box"></div>

          </div>

        </div>

        <div class="project-info">

          <h3>AutoCare</h3>

          <p>
            Automotive service website concept.
          </p>

        </div>

      </article>

    </div>

  </div>

</section>


<section id="services" class="services">

  <div class="container">

    <div class="section-head">

      <div>
        <div class="eyebrow">What I Do</div>
        <h2>Services</h2>
      </div>

    </div>


    <div class="service-grid">

      <div class="service">

        <div class="service-number">01</div>

        <h3>Business Websites</h3>

        <p>
          Professional websites for small businesses,
          services and local brands.
        </p>

      </div>


      <div class="service">

        <div class="service-number">02</div>

        <h3>Mobile-Friendly Design</h3>

        <p>
          Responsive layouts that work across phones,
          tablets and desktop screens.
        </p>

      </div>


      <div class="service">

        <div class="service-number">03</div>

        <h3>Website Improvements</h3>

        <p>
          Clean up an existing website and improve
          its layout, usability and presentation.
        </p>

      </div>

    </div>

  </div>

</section>


<section id="about">

  <div class="container about-grid">

    <div>

      <div class="eyebrow">About</div>

      <h2>
        Simple design. Clear communication. Useful websites.
      </h2>

    </div>


    <div>

      <p>
        ADI WEB STUDIO focuses on creating straightforward,
        professional websites for small businesses.
      </p>

      <p>
        The goal is simple: make the business look trustworthy,
        explain what it offers clearly and make it easy for
        customers to get in touch.
      </p>


      <div class="facts">

        <div class="fact">
          <span>Focus</span>
          <span>Small Businesses</span>
        </div>

        <div class="fact">
          <span>Design</span>
          <span>Clean & Modern</span>
        </div>

        <div class="fact">
          <span>Devices</span>
          <span>Mobile & Desktop</span>
        </div>

        <div class="fact">
          <span>Based</span>
          <span>UAE</span>
        </div>

      </div>

    </div>

  </div>

</section>


<section id="contact" class="contact">

  <div class="container contact-box">

    <div>

      <div class="eyebrow">
        Start a Project
      </div>

      <h2>
        Have a business that needs a website?
      </h2>

      <p>
        Send me a message and tell me what you need.
      </p>

    </div>


    <div class="contact-card">

      <p>
        Email
      </p>

      <a
        class="email"
        href="mailto:adithachamikara29@gmail.com">
        adithachamikara29@gmail.com
      </a>

      <br><br>

      <a
        class="btn"
        href="mailto:adithachamikara29@gmail.com">
        Contact Me
      </a>

    </div>

  </div>

</section>

</main>


<footer>

  <div class="container">

    © 2026 ADI WEB STUDIO. Demo portfolio.

  </div>

</footer>

</div>


<!-- ================= NEXORA ================= -->

<div id="nexora" class="page demo nexora">

  <div class="demo-top">

    <div class="container">

      <button class="back" onclick="showPage('home')">
        ← Back to ADI WEB STUDIO
      </button>

    </div>

  </div>


  <nav class="demo-nav">

    <div class="container demo-nav-inner">

      <div class="demo-logo">
        NEXORA
      </div>

      <div class="demo-links">

        <a href="#nexora-services">Services</a>
        <a href="#nexora-process">Process</a>
        <a href="#nexora-about">About</a>

      </div>

    </div>

  </nav>


  <section class="demo-hero">

    <div class="container">

      <div class="eyebrow">
        Business Solutions
      </div>

      <h1>
        Your business, made simpler.
      </h1>

      <p>
        Practical digital solutions that help small and
        medium-sized businesses organize their operations,
        customers and growth.
      </p>

      <button class="btn" onclick="demoScroll('nexora-services')">
        Explore Services
      </button>

    </div>

  </section>


  <section id="nexora-services" class="demo-section">

    <div class="container">

      <div class="eyebrow">Services</div>

      <h2>What NEXORA provides</h2>


      <div class="demo-grid">

        <div class="demo-card">
          <h3>Operations</h3>
          <p>
            Tools and workflows designed to simplify
            everyday business operations.
          </p>
        </div>

        <div class="demo-card">
          <h3>Customer Management</h3>
          <p>
            Organize customer information and improve
            communication.
          </p>
        </div>

        <div class="demo-card">
          <h3>Digital Growth</h3>
          <p>
            Build a stronger online presence with
            practical digital solutions.
          </p>
        </div>

      </div>

    </div>

  </section>


  <section id="nexora-process" class="demo-section">

    <div class="container">

      <div class="eyebrow">Process</div>

      <h2>How it works</h2>


      <div class="demo-grid">

        <div class="demo-card">
          <h3>01 — Discover</h3>
          <p>
            Understand the business and its requirements.
          </p>
        </div>

        <div class="demo-card">
          <h3>02 — Plan</h3>
          <p>
            Create a clear structure and practical solution.
          </p>
        </div>

        <div class="demo-card">
          <h3>03 — Build</h3>
          <p>
            Turn the plan into a simple, useful digital experience.
          </p>
        </div>

      </div>

    </div>

  </section>


  <section id="nexora-about" class="demo-section">

    <div class="container">

      <div class="eyebrow">About NEXORA</div>

      <h2>Built around practical business needs.</h2>

      <p style="max-width:650px;color:#777;">
        NEXORA is a fictional business concept created by
        ADI WEB STUDIO as a portfolio demonstration.
      </p>

    </div>

  </section>


  <div class="demo-footer">

    <div class="container">

      NEXORA — Fictional portfolio project.

    </div>

  </div>

</div>


<!-- ================= CAFE ================= -->

<div id="cafe" class="page demo cafe">

  <div class="demo-top">

    <div class="container">

      <button class="back" onclick="showPage('home')">
        ← Back to ADI WEB STUDIO
      </button>

    </div>

  </div>


  <nav class="demo-nav">

    <div class="container demo-nav-inner">

      <div class="demo-logo">
        Corner & Co.
      </div>

      <div class="demo-links">

        <a href="#cafe-menu">Menu</a>
        <a href="#cafe-about">About</a>

      </div>

    </div>

  </nav>


  <section class="demo-hero">

    <div class="container">

      <div class="eyebrow">
        Café & Coffee
      </div>

      <h1>
        Good coffee. Good food. Good company.
      </h1>

      <p>
        A relaxed neighbourhood café serving coffee,
        breakfast and simple favourites.
      </p>

      <button
        class="btn"
        onclick="demoScroll('cafe-menu')">
        View Menu
      </button>

    </div>

  </section>


  <section id="cafe-menu" class="demo-section">

    <div class="container">

      <div class="eyebrow">Menu</div>

      <h2>Popular favourites</h2>


      <div class="menu">

        <div class="menu-item">

          <div>
            <strong>Classic Latte</strong>
            <p>Espresso with smooth steamed milk.</p>
          </div>

          <div class="price">AED 16</div>

        </div>


        <div class="menu-item">

          <div>
            <strong>Cappuccino</strong>
            <p>Rich espresso with creamy foam.</p>
          </div>

          <div class="price">AED 15</div>

        </div>


        <div class="menu-item">

          <div>
            <strong>Chicken Sandwich</strong>
            <p>Fresh bread, chicken and house salad.</p>
          </div>

          <div class="price">AED 24</div>

        </div>


        <div class="menu-item">

          <div>
            <strong>Chocolate Cake</strong>
            <p>Soft chocolate cake with a rich finish.</p>
          </div>

          <div class="price">AED 18</div>

        </div>

      </div>

    </div>

  </section>


  <section id="cafe-about" class="demo-section">

    <div class="container">

      <div class="eyebrow">Our Story</div>

      <h2>A local place to slow down.</h2>

      <p style="max-width:650px;color:#777;">
        Corner & Co. is a fictional café concept created by
        ADI WEB STUDIO as a portfolio demonstration.
      </p>

    </div>

  </section>


  <div class="demo-footer">

    <div class="container">

      Corner & Co. — Fictional portfolio project.

    </div>

  </div>

</div>


<!-- ================= AUTOCARE ================= -->

<div id="autocare" class="page demo autocare">

  <div class="demo-top">

    <div class="container">

      <button class="back" onclick="showPage('home')">
        ← Back to ADI WEB STUDIO
      </button>

    </div>

  </div>


  <nav class="demo-nav">

    <div class="container demo-nav-inner">

      <div class="demo-logo">
        AutoCare
      </div>

      <div class="demo-links">

        <a href="#auto-services">Services</a>
        <a href="#auto-about">About</a>

      </div>

    </div>

  </nav>


  <section class="demo-hero">

    <div class="container">

      <div class="eyebrow">
        Automotive Service
      </div>

      <h1>
        Reliable car care without the confus
