

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Garissa County Referral Hospital</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      overflow-x: hidden;
      min-height: 100vh;
      position: relative;
    }

    .background-slideshow {
      position: fixed;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      z-index: -1;
    }

    .background-slideshow img {
      position: absolute;
      width: 100%;
      height: 100%;
      object-fit: cover;
      opacity: 0;
      transition: opacity 2s ease-in-out;
      filter: brightness(1.15);
    }

    .background-slideshow img.active {
      opacity: 1;
    }

    header {
      background-color: rgba(0, 0, 0, 0.75);
      color: white;
      padding: 1rem;
      text-align: center;
      z-index: 5;
    }

    header img {
      width: 200px;
      vertical-align: middle;
    }

    nav {
      background-color: rgba(0, 87, 122, 0.95);
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 0.5rem;
      z-index: 5;
    }

    nav ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin: 0;
      padding: 0;
    }

    nav ul li {
      position: relative;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      padding: 0.5rem 1rem;
      display: block;
      font-weight: bold;
    }

    nav ul li ul {
      display: none;
      position: absolute;
      top: 100%;
      left: 0;
      background: rgba(0, 87, 122, 0.95);
      padding: 0;
      margin: 0;
      list-style: none;
      z-index: 6;
    }

    nav ul li:hover > ul {
      display: block;
    }

    nav ul li ul li ul {
      display: none;
      position: absolute;
      top: 0;
      left: 100%;
      background: rgba(0, 87, 122, 0.95);
    }

    nav ul li ul li:hover ul {
      display: block;
    }

    .spacer {
      height: 450px;
    }

    .content {
      padding: 2rem;
      color: white;
      text-align: center;
    }

    .stats, .management {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
      margin: 4rem auto;
      max-width: 1000px;
      background: rgba(0, 87, 122, 0.9);
      border-radius: 12px;
      padding: 3rem;
      border: 2px solid white;
    }

    .stat, .manager {
      flex: 1 1 250px;
      text-align: center;
      font-size: 1.2rem;
      color: #fff;
    }

    .manager img {
      width: 150px;
      height: 150px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 1rem;
      border: 3px solid white;
    }

    nav ul li > a::after {
      content: ' ▼';
      font-size: 0.6em;
      margin-left: 4px;
    }

    nav ul li:not(:hover) > a:only-child::after {
      content: '';
    }

    nav ul li ul li > a::after {
      content: '';
    }

    .toggle-submenu > ul {
      display: block !important;
    }

    /* --- Beautiful Footer Styling --- */
    footer {
      background: linear-gradient(to right, #003344, #005566);
      color: #f1f1f1;
      padding: 3rem 2rem;
      text-align: center;
      font-size: 1rem;
      line-height: 1.6;
    }

    footer p {
      margin: 0.4rem 0;
    }

    footer p strong {
      color: #ffcc00;
    }

    footer .footer-highlight {
      font-size: 1.1rem;
      font-weight: bold;
      color: #ffffff;
      margin-top: 1.5rem;
    }

    footer hr {
      border: none;
      height: 1px;
      background-color: #ffffff33;
      margin: 1.5rem 0;
    }

    footer a {
      color: #ffcc00;
      text-decoration: none;
    }

    footer a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
    <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Background Slideshow</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body, html {
      height: 100%;
      font-family: Arial, sans-serif;
      position: relative;
    }

    .slideshow-container {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100vh;
      overflow: hidden;
      z-index: -1;
    }

    .slideshow-slide {
      position: absolute;
      width: 100%;
      height: 100%;
      background-size: cover;
      background-position: center;
      opacity: 0;
      transition: opacity 1s ease-in-out;
    }

    .slideshow-slide.active {
      opacity: 0.9; /* Adjust to make it look like a watermark */
    }
  </style>
</head>
<body>

  <div class="slideshow-container">
    <div class="slideshow-slide" style="background-image: url('slide8.jpg');"></div>
    <div class="slideshow-slide" style="background-image: url('slide2.jpg');"></div>
    <div class="slideshow-slide" style="background-image: url('slide3.jpg');"></div>
    <div class="slideshow-slide" style="background-image: url('Slide7.jpg');"></div>
    <div class="slideshow-slide" style="background-image: url('slide6.jpg.jpg');"></div>
    <div class="slideshow-slide" style="background-image: url('slide10.jpg');"></div>
  </div>

  <script>
    const slides = document.querySelectorAll('.slideshow-slide');
    let index = 0;

    function showSlide(i) {
      slides.forEach((slide, idx) => {
        slide.classList.remove('active');
        if (idx === i) slide.classList.add('active');
      });
    }

    showSlide(index);

    setInterval(() => {
      index = (index + 1) % slides.length;
      showSlide(index);
    }, 2000);
  </script>

</body>
</html>

  <header>
    <img src="GCRH.LOGO.png" alt="Hospital Logo" />
    <h1>Garissa County Referral Hospital</h1>
  </header>

  </header>

<nav class="main-nav">
  <ul class="nav-menu">
    <li><a href="#">Home</a></li>
    <li>
      <a href="#">Our Services</a>
      <ul class="dropdown">
        <li>
          <a href="#">Clinical Services</a>
          <ul class="dropdown">
            <li><a href="#">Surgical Services</a></li>
            <li><a href="#">Medical Services</a></li>
            <li><a href="#">Diagnostic Services</a></li>
            <li><a href="#">Pharmaceutical Services</a></li>
            <li><a href="#">Nursing Services</a></li>
            <li><a href="#">Specialized Clinics</a></li>
            <li><a href="#">Schedule</a></li>
          </ul>
        </li>
        <li><a href="#">Centers Of Excellence</a></li>
        <li><a href="#">Medical Research & Programs</a></li>
        <li><a href="#">Patient Affairs</a></li>
        <li><a href="#">Covid-19 Centre</a></li>
      </ul>
    <li class="nav-item dropdown">
  <a href="#" class="nav-link">About Us</a>
  <ul class="dropdown-menu">
    <li><a href="#history" class="dropdown-item">Our History</a></li>
    <li><a href="#whoweare" class="dropdown-item">Who We Are</a></li>
    <li><a href="#directorates" class="dropdown-item">Directorates</a></li>
    <li><a href="#management" class="dropdown-item">Management</a></li>
    <li><a href="#milestones" class="dropdown-item">Milestones</a></li>
    <li><a href="#careers" class="dropdown-item">Careers</a></li>
    <li><a href="#tenders" class="dropdown-item">Tenders</a></li>
  </ul>
</li>
     <li class="nav-item dropdown">
  <a href="#" class="nav-link">Departments</a>
  <ul class="dropdown-menu">
    <li><a href="#">Clinical Services Department</a></li>
    <li><a href="#">Nursing Services Department</a></li>
    <li><a href="#">Pharmaceutical Services Department</a></li>
    <li><a href="#">Diagnostic Services Department</a></li>
    <li><a href="#">Public Health & Preventive Services</a></li>
    <li><a href="#">Health Information Management</a></li>
    <li><a href="#">ICT Department</a></li>
    <li><a href="#">Admin & HR Department</a></li>
    <li><a href="#">Finance & Accounts</a></li>
    <li><a href="#">Procurement & Supply Chain</a></li>
    <li><a href="#">Engineering & Maintenance</a></li>
    <li><a href="#">Support Services</a></li>
    <li><a href="#">Media & Communication</a></li>
  </ul>
</li>
  <a href="#">Gallery / Media Center</a>
  <ul class="dropdown">
    <li><a href="#">Photos</a></li>
    <li><a href="#">Videos</a></li>
    <li><a href="#">Press Releases</a></li>
    <li>
      <a href="#">Newsletters</a>
      <ul class="dropdown">
        <li><a href="#">Monthly Reports</a></li>
        <li><a href="#">Blogs</a></li> <!-- New link added here -->
      </ul>
    </li>
  </ul>
</li>
  </ul>
</nav>

  <div class="spacer"></div>

 <!-- Statistics Section -->
<div class="content" style="background: linear-gradient(135deg, #f0f8ff, #e6f2ff); padding: 80px 20px;">
  <h2 style="text-align: center; color: #063970; font-size: 36px; font-weight: 700; margin-bottom: 60px; letter-spacing: 1px;">
    Hospital At a Glance
  </h2>
  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 40px;">
    
    <!-- Stat Box -->
    <div style="flex: 1 1 220px; max-width: 260px; background: #fff; padding: 35px 25px; border-radius: 20px; text-align: center; box-shadow: 0 10px 25px rgba(0,0,0,0.08); transition: transform 0.3s;">
      <div style="font-size: 45px; color: #0096c7;">🛏️</div>
      <h3 style="margin-top: 20px; font-size: 20px; color: #063970; font-weight: 600;">Bed Capacity</h3>
      <p style="font-size: 30px; color: #00b4d8; font-weight: 700; margin-top: 10px;">500</p>
    </div>

    <!-- Stat Box -->
    <div style="flex: 1 1 220px; max-width: 260px; background: #fff; padding: 35px 25px; border-radius: 20px; text-align: center; box-shadow: 0 10px 25px rgba(0,0,0,0.08); transition: transform 0.3s;">
      <div style="font-size: 45px; color: #0096c7;">👩‍⚕️</div>
      <h3 style="margin-top: 20px; font-size: 20px; color: #063970; font-weight: 600;">Employees</h3>
      <p style="font-size: 30px; color: #00b4d8; font-weight: 700; margin-top: 10px;">500</p>
    </div>

    <!-- Stat Box -->
    <div style="flex: 1 1 220px; max-width: 260px; background: #fff; padding: 35px 25px; border-radius: 20px; text-align: center; box-shadow: 0 10px 25px rgba(0,0,0,0.08); transition: transform 0.3s;">
      <div style="font-size: 45px; color: #0096c7;">📅</div>
      <h3 style="margin-top: 20px; font-size: 20px; color: #063970; font-weight: 600;">Years of Service</h3>
      <p style="font-size: 30px; color: #00b4d8; font-weight: 700; margin-top: 10px;">60</p>
    </div>

    <!-- Stat Box -->
    <div style="flex: 1 1 220px; max-width: 260px; background: #fff; padding: 35px 25px; border-radius: 20px; text-align: center; box-shadow: 0 10px 25px rgba(0,0,0,0.08); transition: transform 0.3s;">
      <div style="font-size: 45px; color: #0096c7;">🏥</div>
      <h3 style="margin-top: 20px; font-size: 20px; color: #063970; font-weight: 600;">Specialized Clinics</h3>
      <p style="font-size: 30px; color: #00b4d8; font-weight: 700; margin-top: 10px;">22</p>
    </div>

  </div>

</div>

   <!-- Management Section -->
<div style="background: #d5d7da; padding: 80px 20px;">
  <h2 style="text-align: center; font-size: 36px; color: #0a4275; margin-bottom: 60px; font-weight: bold;">Meet Our Leadership</h2>
  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 40px;">
    
    <div style="background: #ffffff; padding: 20px; border-radius: 16px; width: 300px; box-shadow: 0 12px 24px rgba(0, 0, 0, 0.08); text-align: center; transition: transform 0.3s ease, box-shadow 0.3s ease;">
      <img src="chairman.png" alt="Bashir Gure Gedi" style="width: 100%; height: 360px; object-fit: cover; border-radius: 12px; margin-bottom: 20px;" />
      <h3 style="margin-bottom: 10px; font-size: 22px; color: #0a4275;">Bashir Gure Gedi</h3>
      <p style="font-size: 16px; color: #333;">Chair, Board of Management</p>
    </div>

    <div style="background: #ffffff; padding: 20px; border-radius: 16px; width: 300px; box-shadow: 0 12px 24px rgba(0, 0, 0, 0.08); text-align: center; transition: transform 0.3s ease, box-shadow 0.3s ease;">
      <img src="ceo.png" alt="Mahat Salah Sheikh" style="width: 100%; height: 360px; object-fit: cover; border-radius: 12px; margin-bottom: 20px;" />
      <h3 style="margin-bottom: 10px; font-size: 22px; color: #0a4275;">Mahat Salah Sheikh</h3>
      <p style="font-size: 16px; color: #333;">Chief Executive Officer</p>
    </div>

    <div style="background: #ffffff; padding: 20px; border-radius: 16px; width: 300px; box-shadow: 0 12px 24px rgba(0, 0, 0, 0.08); text-align: center; transition: transform 0.3s ease, box-shadow 0.3s ease;">
      <img src="buro.png" alt="Dr Hussein Buro" style="width: 100%; height: 360px; object-fit: cover; border-radius: 12px; margin-bottom: 20px;" />
      <h3 style="margin-bottom: 10px; font-size: 22px; color: #0a4275;">Dr Hussein Buro</h3>
      <p style="font-size: 16px; color: #333;">Director - Clinical Services</p>
    </div>

  </div>
</div>


 <!-- ...everything above remains unchanged... -->

 <!-- Our Partners Section -->
<section style="background-color: #f8f9fa; padding: 60px 20px; font-family: Arial, sans-serif;">
  <div style="max-width: 1200px; margin: auto; text-align: center;">
    <h2 style="color: #0a4275; font-size: 32px; margin-bottom: 40px;">Our Trusted Partners</h2>
    <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 40px;">

      <a href="https://garissa.go.ke" target="_blank" style="text-decoration: none;">
        <div style="flex: 1 1 180px; max-width: 200px; transition: transform 0.3s;">
          <img src="garissa logo.png" alt="Garissa County" style="width:100%; height:auto; border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.1);">
          <p style="margin-top: 15px; font-weight: bold; color: #333;">Garissa County</p>
        </div>
      </a>

      <a href="https://www.icrc.org" target="_blank" style="text-decoration: none;">
        <div style="flex: 1 1 180px; max-width: 200px; transition: transform 0.3s;">
          <img src="ICRC.png" alt="ICRC" style="width:100%; height:auto; border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.1);">
          <p style="margin-top: 15px; font-weight: bold; color: #333;">ICRC</p>
        </div>
      </a>

      <a href="https://www.kmtc.ac.ke" target="_blank" style="text-decoration: none;">
        <div style="flex: 1 1 180px; max-width: 200px; transition: transform 0.3s;">
          <img src="KMTC.png" alt="KMTC" style="width:100%; height:auto; border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.1);">
          <p style="margin-top: 15px; font-weight: bold; color: #333;">KMTC</p>
        </div>
      </a>

     <a href="https://www.amref.org" target="_blank" style="text-decoration: none;">
        <div style="flex: 1 1 180px; max-width: 200px; transition: transform 0.3s;">
          <img src="AMREF.png" alt="Amref" style="width:100%; height:auto; border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.1);">
          <p style="margin-top: 15px; font-weight: bold; color: #333;">Amref Health Africa</p>
        </div>
      </a>
      <a href="https://www.nepcollege.ac.ke" target="_blank" style="text-decoration: none;">
  <div style="flex: 1 1 180px; max-width: 200px; transition: transform 0.3s;">
    <img src="nep_collage-removebg-preview.png" alt="NEP College" style="width:100%; height:auto; border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.1);">
    <p style="margin-top: 15px; font-weight: bold; color: #333;">NEP College</p>
  </div>
</a>

    </div>
  </div>
</section>


<!-- Services Section -->
<div class="content" style="background-color: #f8fafc; padding: 60px 20px;">
  <h2 style="text-align: center; color: #0a4275; font-size: 36px; margin-bottom: 40px; font-weight: bold;">Our Services</h2>
  
  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 40px;">
    <!-- Service Card -->
    <div style="max-width: 320px; background: #fff; padding: 25px; border-radius: 15px; box-shadow: 0 10px 20px rgba(0,0,0,0.08); transition: transform 0.3s, box-shadow 0.3s;">
      <h3 style="color: #0a4275; font-size: 22px; margin-bottom: 15px;">Surgical</h3>
      <p style="color: #555; line-height: 1.6;">GCRH conducts numerous major and minor surgeries and brings together multidisciplinary faculty and staff to enhance patient care and research.</p>
    </div>

    <!-- Service Card -->
    <div style="max-width: 320px; background: #fff; padding: 25px; border-radius: 15px; box-shadow: 0 10px 20px rgba(0,0,0,0.08); transition: transform 0.3s, box-shadow 0.3s;">
      <h3 style="color: #0a4275; font-size: 22px; margin-bottom: 15px;">Medical</h3>
      <p style="color: #555; line-height: 1.6;">We manage services including Pediatrics, Cardiology, Mental Health, Nutrition, Oncology, Renal, Infectious Diseases, Diabetes, and more.</p>
    </div>

    <!-- Service Card -->
    <div style="max-width: 320px; background: #fff; padding: 25px; border-radius: 15px; box-shadow: 0 10px 20px rgba(0,0,0,0.08); transition: transform 0.3s, box-shadow 0.3s;">
      <h3 style="color: #0a4275; font-size: 22px; margin-bottom: 15px;">Diagnostics</h3>
      <p style="color: #555; line-height: 1.6;">Radiology, laboratory testing, farewell services, and health information systems support our commitment to clinical excellence.</p>
    </div>

    <!-- Service Card -->
    <div style="max-width: 320px; background: #fff; padding: 25px; border-radius: 15px; box-shadow: 0 10px 20px rgba(0,0,0,0.08); transition: transform 0.3s, box-shadow 0.3s;">
      <h3 style="color: #0a4275; font-size: 22px; margin-bottom: 15px;">Pharmaceutical</h3>
      <p style="color: #555; line-height: 1.6;">Our pharmaceutical services include clinical pharmacy, pharmacovigilance, drug information, and in-house production of medications.</p>
    </div>
  </div>

  <!-- CTA Button -->
  <div style="text-align: center; margin-top: 40px;">
    <a href="#" style="background-color: #0a4275; color: white; padding: 14px 30px; border-radius: 30px; text-decoration: none; font-weight: bold; font-size: 16px; transition: background-color 0.3s;">SEE MORE SERVICES</a>
  </div>
</div>

<!-- Hover effect using inline <style> -->
<style>
  .content div:hover {
    transform: translateY(-8px);
    box-shadow: 0 15px 25px rgba(0, 0, 0, 0.12);
  }
</style>


 <!-- Social Media Channels Section -->
<div class="content" style="background: linear-gradient(to bottom right, rgba(135,206,250,0.3), rgba(70,130,180,0.4)), url('https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0?auto=format&fit=crop&w=1470&q=80'); background-size: cover; background-position: center; padding: 4rem 1.5rem; border-radius: 20px; margin-top: 3rem; box-shadow: 0 12px 30px rgba(0,0,0,0.3); backdrop-filter: blur(6px);">

  <h2 style="color: #ffffff; text-align: center; font-size: 2.75rem; margin-bottom: 3rem; font-weight: 700; letter-spacing: 1.2px; text-transform: uppercase; text-shadow: 0 2px 4px rgba(0,0,0,0.4);">
    Connect With Us
  </h2>

  <div class="social-grid" style="display: flex; justify-content: center; gap: 2.5rem; flex-wrap: wrap;">

    <div class="social-card">
      <img src="facebook logo.jpg"Facebook Logo">
      <a href="https://facebook.com" target="_blank">Facebook</a>
    </div>

    <div class="social-card">
      <img src="x logo.png" alt="Twitter Logo">
      <a href="https://twitter.com" target="_blank">X (Twitter)</a>
    </div>

    <div class="social-card">
      <img src="youtube.png" alt="YouTube Logo">
      <a href="https://youtube.com" target="_blank">YouTube</a>
    </div>

    <div class="social-card">
      <img src="news.jpg" alt="News">
      <a href="https://rgk.co.ke/top-stories/34282/garissa-referral-hospital-secures-sustainable-drug-supply-system-ceo-mahat" target="_blank">News Portal</a>
    </div>

  </div>
</div>

<style>
  .social-card {
    background-color: rgba(255, 255, 255, 0.15);
    padding: 2rem 1.5rem;
    border-radius: 16px;
    text-align: center;
    transition: all 0.3s ease;
    width: 180px;
    backdrop-filter: blur(4px);
    box-shadow: 0 8px 18px rgba(0,0,0,0.2);
  }

  .social-card img {
    width: 60px;
    height: auto;
    margin-bottom: 1rem;
    transition: transform 0.3s ease;
  }

  .social-card a {
    color: #ffffff;
    font-size: 1.2rem;
    font-weight: 600;
    text-decoration: none;
    display: inline-block;
    transition: color 0.3s ease, text-decoration 0.3s ease;
  }

  .social-card:hover {
    transform: translateY(-8px);
    background-color: rgba(255, 255, 255, 0.22);
    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.3);
  }

  .social-card:hover img {
    transform: scale(1.15);
  }

  .social-card a:hover {
    color: #00e5ff;
    text-decoration: underline;
  }

  /* Optional: Slight bounce on hover */
  .social-card {
    transition: transform 0.3s ease-in-out;
  }
</style>

 <!-- Testimonials Section -->
<section class="testimonials-section" style="background: rgba(255, 255, 255, 0.3); backdrop-filter: blur(10px); padding: 5rem 1.5rem; color: #1c1c1c; text-align: center; border-radius: 20px; margin-top: 3rem; box-shadow: 0 10px 30px rgba(0,0,0,0.15);">
  <h2 style="font-size: 2.5rem; font-weight: 700; margin-bottom: 3rem; letter-spacing: 1px; color: #003c2f;">What Our Clients Say</h2>

  <div class="testimonial-slider" style="position: relative; max-width: 900px; margin: auto; overflow: hidden; border-radius: 16px;">
    <div class="testimonial-track" id="testimonialTrack" style="display: flex; transition: transform 0.8s ease;">
      <!-- Testimonial 1 -->
      <div class="testimonial-card">
        <p><strong style="color: #0d6efd;">@devis mumo</strong><br/>
        <em>device mumo</em><br/>
        “Congratulations and may God bless you.”</p>
      </div>
      <!-- Testimonial 2 -->
      <div class="testimonial-card">
        <p><strong style="color: #0d6efd;">@Halima jelle</strong><br/>
        <em>halima jelle jamac</em><br/>
        “Having gone to different hospitals and not getting help, we landed at GCRH. My son was admitted and had major surgery. After staying in ward 1E and receiving amazing follow-up care, our miracle boy is now in his final year of university. The oncology doctors are the best.”</p>
      </div>
      <!-- Testimonial 3 -->
      <div class="testimonial-card">
        <p><strong style="color: #0d6efd;">@Daud Hareth</strong><br/>
         <em>daud hareth</em><br/>
        “We value your service, keep up!”</p>
      </div>
      <!-- Testimonial 4 -->
      <div class="testimonial-card">
        <p><strong style="color: #0d6efd;">ramazan@254</strong><br/>
        “I just want to thank God for the treatment I received. Doctors and nurses went out of their way. Be blessed beyond expectations.”</p>
      </div>
      <!-- Testimonial 5 -->
      <div class="testimonial-card">
        <p><strong style="color: #0d6efd;">betrice awour</strong><br/>
        “I appreciate your medics so much. My son is back to normal. ENT team, thank you!”</p>
      </div>
      <!-- Testimonial 6 -->
      <div class="testimonial-card">
        <p><strong style="color: #0d6efd;">diriye@26</strong><br/>
        “The best hospital in Kenya.”</p>
      </div>
    </div>
  </div>
</section>

<style>
  .testimonial-card {
    min-width: 100%;
    background: rgba(255, 255, 255, 0.8);
    color: #222;
    padding: 2rem;
    border-radius: 12px;
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.15);
    transition: transform 0.5s ease;
    font-size: 1.1rem;
    line-height: 1.7;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }

  .testimonial-card:hover {
    transform: scale(1.03);
  }

  @keyframes slideTestimonial {
    0% { transform: translateX(0); }
    20% { transform: translateX(0); }
    25% { transform: translateX(-100%); }
    45% { transform: translateX(-100%); }
    50% { transform: translateX(-200%); }
    70% { transform: translateX(-200%); }
    75% { transform: translateX(-300%); }
    95% { transform: translateX(-300%); }
    100% { transform: translateX(0); }
  }

  #testimonialTrack {
    animation: slideTestimonial 35s infinite ease-in-out;
  }
   </div>
    </div>
  </div>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Garissa County Referral Hospital</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
    }

    footer {
      background-color: #003366;
      color: #ffffff;
      padding: 60px 20px 30px;
    }

    .footer-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      max-width: 1200px;
      margin: auto;
    }

    .footer-col {
      flex: 1 1 300px;
      margin: 20px;
    }

    .footer-col h4 {
      font-size: 22px;
      margin-bottom: 20px;
      border-bottom: 2px solid #ffffff44;
      padding-bottom: 8px;
    }

    .footer-col p, .footer-col ul li {
      font-size: 17px;
      line-height: 1.6;
    }

    .footer-col ul {
      list-style: none;
      padding: 0;
    }

    .footer-col ul li {
      margin: 12px 0;
    }

    .footer-col ul li a {
      color: #ffffff;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .footer-col ul li a:hover {
      text-decoration: underline;
      color: #ffcc00;
    }

    .footer-bottom {
      text-align: center;
      padding: 30px 0 0;
      margin-top: 40px;
      border-top: 1px solid #ffffff33;
      font-size: 16px;
      color: #cccccc;
    }

    @media (max-width: 768px) {
      .footer-container {
        flex-direction: column;
        align-items: center;
      }

      .footer-col {
        text-align: center;
      }
    }
  </style>
</head>
<body>

  <!-- Footer -->
  <footer>
    <div class="footer-container">
      <!-- Contact Info -->
      <div class="footer-col">
        <h4>Contact Us</h4>
        <p><strong>Garissa County Referral Hospital</strong></p>
        <p>P.O. Box 29 - 70100, Garissa, Kenya</p>
        <p>Email: garissapgh@yahoo.com</p>
        <p>Phone: +254 720 705 683</p>
      </div>

      <!-- Quick Links -->
<div class="footer-col">
  <h4>Quick Links</h4>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Departments</a></li>
    <li><a href="#">Doctors</a></li>
    <li><a href="#">Contact</a></li>
    <li><a href="https://webmail.healthgarissa.go.ke" target="_blank">Staff Mail</a></li>
    <li><a href="https://afyayangu.go.ke/#/registration" target="_blank">Register SHA</a></li>
  </ul>
</div>

      <!-- Mission & Vision -->
      <div class="footer-col">
        <h4>Our Vision</h4>
        <p>A centre of excellence in provision of accessible, affordable and socially acceptable quality health care services in the region and beyond.</p>
        <h4>Our Mission</h4>
        <p>To build a progressive, responsive and sustainable health system offering promotive, preventive, curative and rehabilitative services.</p>
      </div>

      <!-- Core Values -->
      <div class="footer-col">
        <h4>Core Values</h4>
        <ul>
          <li>Efficiency & Effectiveness</li>
          <li>Compassion</li>
          <li>Inclusivity & Equity</li>
          <li>Professionalism</li>
          <li>Accountability & Integrity</li>
          <li>Innovation</li>
          <li>Team Work</li>
        </ul>
      </div>
    </div>

    <div class="footer-bottom">
      &copy; 2025 Garissa County Referral Hospital. All Rights Reserved.
    </div>
  </footer>

</body>
</html>

