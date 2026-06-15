<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>یحیی طاهری — برنامه‌نویس حرفه‌ای پایتون و اکسل</title>

  <!-- فونت وزیر -->
  <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn/Vazirmatn-font-face.css" rel="stylesheet" />

  <!-- آیکون‌ها -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet" />

  <!-- Swiper CSS -->
  <link
    rel="stylesheet"
    href="https://cdn.jsdelivr.net/npm/swiper@9/swiper-bundle.min.css"
  />

  <style>
    :root {
      --clr-primary: #22d3ee;
      --clr-primary-dark: #0891b2;
      --clr-bg-dark: #0a1f3d;
      --clr-bg-light: #f5f7fa;
      --clr-text-dark: #e0e7ff;
      --clr-text-light: #1e293b;
      --clr-glass-bg: rgba(255 255 255 / 0.12);
      --clr-glass-bg-dark: rgba(0 0 0 / 0.25);
      --shadow-glass: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
      --border-glass: 1px solid rgba(255, 255, 255, 0.18);
    }
    * {
      margin: 0; padding: 0; box-sizing: border-box;
      scroll-behavior: smooth;
      user-select: none;
    }
    body {
      font-family: 'Vazirmatn', sans-serif;
      background: linear-gradient(270deg, #0a1f3d, #022c5a, #0a1f3d);
      background-size: 600% 600%;
      animation: gradientBG 15s ease infinite;
      color: var(--clr-text-dark);
      min-height: 100vh;
      direction: rtl;
      overflow-x: hidden;
      transition: background-color 0.4s, color 0.4s;
      position: relative;
    }
    body.light {
      background: var(--clr-bg-light);
      color: var(--clr-text-light);
    }
    @keyframes gradientBG {
      0% {background-position:0% 50%}
      50% {background-position:100% 50%}
      100% {background-position:0% 50%}
    }

    /* نوار ناوبری */
    nav {
      position: fixed;
      top: 0; left: 0; right: 0;
      background: var(--clr-glass-bg);
      backdrop-filter: blur(12px);
      box-shadow: 0 2px 15px rgba(0,0,0,0.3);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      z-index: 1100;
      transition: background-color 0.3s;
    }
    body.light nav {
      background: var(--clr-glass-bg-dark);
      box-shadow: 0 2px 15px rgba(0,0,0,0.1);
    }
    nav .logo {
      font-size: 1.8rem;
      font-weight: 900;
      color: var(--clr-primary);
      cursor: default;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 1.8rem;
    }
    nav ul li a {
      font-weight: 600;
      font-size: 1rem;
      color: var(--clr-text-dark);
      padding-bottom: 4px;
      border-bottom: 2px solid transparent;
      transition: all 0.3s ease;
      cursor: pointer;
    }
    body.light nav ul li a {
      color: var(--clr-text-light);
    }
    nav ul li a:hover,
    nav ul li a.active {
      color: var(--clr-primary);
      border-bottom-color: var(--clr-primary);
    }

    /* انیمیشن */
    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* پروفایل کنار صفحه ثابت */
    #profile-fixed {
      position: fixed;
      top: 40%;
      right: 0;
      background: var(--clr-glass-bg);
      backdrop-filter: blur(12px);
      padding: 1rem;
      border-radius: 20px 0 0 20px;
      box-shadow: var(--shadow-glass);
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 0.8rem;
      z-index: 1050;
      transition: background-color 0.3s;
    }
    body.light #profile-fixed {
      background: var(--clr-glass-bg-dark);
    }
    #profile-fixed img {
      width: 70px;
      border-radius: 50%;
      border: 3px solid var(--clr-primary);
      cursor: pointer;
      transition: transform 0.3s ease;
    }
    #profile-fixed img:hover {
      transform: scale(1.15);
    }
    #profile-fixed a {
      color: var(--clr-primary);
      font-size: 1.3rem;
      transition: color 0.3s ease;
      cursor: pointer;
    }
    #profile-fixed a:hover {
      color: var(--clr-primary-dark);
    }

    /* بخش‌ها با گرید و گلاس */
    section {
      max-width: 1000px;
      margin: 80px auto;
      padding: 2rem 1rem;
      border-radius: 20px;
      background: var(--clr-glass-bg);
      backdrop-filter: blur(18px);
      -webkit-backdrop-filter: blur(18px);
      box-shadow: var(--shadow-glass);
      border: var(--border-glass);
      color: var(--clr-text-dark);
      transition: background-color 0.3s, color 0.3s;
    }
    body.light section {
      background: var(--clr-glass-bg-dark);
      color: var(--clr-text-light);
    }
    section h2 {
      font-size: 2.8rem;
      font-weight: 900;
      color: var(--clr-primary);
      margin-bottom: 1.5rem;
      text-align: center;
      text-shadow: 0 0 15px rgba(34, 211, 238, 0.6);
      user-select: text;
    }

    /* درباره من */
    #about {
      display: grid;
      grid-template-columns: 250px 1fr;
      gap: 3rem;
      align-items: center;
    }
    #about img {
      width: 100%;
      border-radius: 20px;
      box-shadow: var(--shadow-glass);
      user-select: none;
      transition: transform 0.3s ease;
      cursor: default;
    }
    #about img:hover {
      transform: scale(1.05);
    }
    #about p {
      font-size: 1.2rem;
      line-height: 1.6;
    }

    /* مهارت‌ها با نمودار دایره‌ای SVG */
    #skills {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(140px,1fr));
      gap: 2.5rem;
      justify-items: center;
    }
    .skill-circle {
      position: relative;
      width: 140px;
      height: 140px;
      cursor: default;
    }
    svg circle {
      fill: none;
      stroke-width: 12;
      stroke-linecap: round;
      transform: rotate(-90deg);
      transform-origin: 50% 50%;
      transition: stroke-dashoffset 1.6s ease;
    }
    .skill-bg {
      stroke: #ddd;
    }
    .skill-progress {
      stroke: var(--clr-primary);
      stroke-dasharray: 339.292; /* circumference */
      stroke-dashoffset: 339.292;
    }
    .skill-text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -55%);
      font-weight: 900;
      font-size: 1.4rem;
      color: var(--clr-primary);
      user-select: text;
    }
    .skill-name {
      text-align: center;
      margin-top: 0.8rem;
      font-weight: 600;
      color: var(--clr-text-dark);
      user-select: text;
    }
    body.light .skill-name {
      color: var(--clr-text-light);
    }

    /* خدمات */
    #services {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
    }
    .service-card {
      flex: 1 1 280px;
      background: var(--clr-bg-dark);
      color: var(--clr-text-dark);
      padding: 2rem 1.5rem;
      border-radius: 20px;
      box-shadow: 0 4px 35px rgba(34, 211, 238, 0.4);
      display: flex;
      flex-direction: column;
      align-items: center;
      transition: transform 0.3s ease, background-color 0.3s ease;
      cursor: default;
      user-select: none;
      text-align: center;
    }
    body.light .service-card {
      background: var(--clr-bg-light);
      color: var(--clr-text-light);
      box-shadow: 0 4px 35px rgba(0, 0, 0, 0.15);
    }
    .service-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 45px var(--clr-primary);
    }
    .service-card i {
      font-size: 4.2rem;
      margin-bottom: 1rem;
      color: var(--clr-primary);
      transition: color 0.3s ease;
    }

    /* نمونه کارها */
    #projects {
      position: relative;
    }
    .swiper {
      padding-bottom: 3rem;
    }
    .project-img {
      width: 100%;
      height: 180px;
      border-radius: 20px;
      object-fit: cover;
      filter: brightness(0.85);
      transition: filter 0.3s ease;
      user-select: none;
      cursor: pointer;
    }
    .project-img:hover {
      filter: brightness(1);
      transform: scale(1.05);
    }
    .project-title {
      margin-top: 0.8rem;
      font-weight: 700;
      font-size: 1.2rem;
      color: var(--clr-primary);
      user-select: text;
    }
    .project-desc {
      font-size: 1rem;
      color: var(--clr-text-dark);
      margin: 0.4rem 0 1rem 0;
      user-select: text;
    }
    .project-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      justify-content: center;
      user-select: none;
    }
    .tag {
      background: var(--clr-primary);
      color: #031124;
      font-weight: 700;
      font-size: 0.75rem;
      padding: 3px 10px;
      border-radius: 100px;
      user-select: none;
      cursor: default;
      transition: background-color 0.3s ease;
    }
    .tag:hover {
      background-color: var(--clr-primary-dark);
    }

    /* نظرات */
    #testimonials {
      max-width: 700px;
      margin: 0 auto;
      padding-top: 1rem;
    }
    .testimonial-slide {
      font-style: italic;
      font-size: 1.1rem;
      color: var(--clr-text-dark);
      padding: 1rem 2rem;
      border-radius: 15px;
      box-shadow: var(--shadow-glass);
      background: var(--clr-glass-bg);
      user-select: text;
    }
    body.light .testimonial-slide {
      background: var(--clr-glass-bg-dark);
      color: var(--clr-text-light);
    }
    .testimonial-author {
      margin-top: 1rem;
      font-weight: 900;
      font-size: 1rem;
      color: var(--clr-primary);
      text-align: left;
      user-select: text;
    }

    /* تماس */
    #contact {
      max-width: 600px;
      margin: 0 auto 5rem;
    }
    #contact form {
      display: flex;
      flex-direction: column;
      gap: 1.1rem;
      user-select: none;
    }
    #contact label {
      font-weight: 700;
      font-size: 1rem;
      user-select: text;
    }
    #contact input,
    #contact textarea {
      font-family: 'Vazirmatn', sans-serif;
      padding: 0.7rem 1rem;
      border-radius: 12px;
      border: 2px solid var(--clr-primary);
      outline-offset: 3px;
      font-size: 1rem;
      resize: vertical;
      transition: border-color 0.3s ease;
      user-select: text;
    }
    #contact input:focus,
    #contact textarea:focus {
      border-color: var(--clr-primary-dark);
    }
    #contact button {
      margin-top: 1rem;
      background: var(--clr-primary);
      color: #031124;
      font-weight: 800;
      font-size: 1.2rem;
      border-radius: 40px;
      padding: 0.9rem 0;
      border: none;
      cursor: pointer;
      box-shadow: 0 8px 30px var(--clr-primary);
      transition: background-color 0.3s ease, box-shadow 0.3s ease;
      user-select: none;
    }
    #contact button:hover {
      background: var(--clr-primary-dark);
      box-shadow: 0 12px 45px var(--clr-primary-dark);
    }
    #contact-status {
      margin-top: 0.8rem;
      font-weight: 600;
      text-align: center;
      user-select: none;
    }
    #contact-status.success {
      color: #4ade80;
    }
    #contact-status.error {
      color: #f87171;
    }

    /* دکمه بازگشت به بالا */
    #backToTop {
      position: fixed;
      bottom: 25px;
      left: 25px;
      background: var(--clr-primary);
      color: #031124;
      border: none;
      padding: 0.5rem 0.8rem;
      font-size: 1.6rem;
      border-radius: 50%;
      cursor: pointer;
      box-shadow: 0 8px 30px var(--clr-primary);
      display: none;
      z-index: 1200;
      user-select: none;
      transition: background-color 0.3s ease;
    }
    #backToTop:hover {
      background: var(--clr-primary-dark);
    }

    /* دکمه تغییر تم */
    #toggleMode {
      background: none;
      border: none;
      cursor: pointer;
      font-size: 1.5rem;
      color: var(--clr-primary);
      user-select: none;
      transition: color 0.3s ease;
    }
    #toggleMode:hover {
      color: var(--clr-primary-dark);
    }

    /* Media Queries */
    @media (max-width: 900px) {
      #about {
        grid-template-columns: 1fr;
        text-align: center;
      }
      #about img {
        margin: 0 auto 2rem auto;
        max-width: 300px;
      }
      nav ul {
        gap: 1rem;
      }
      #services {
        flex-direction: column;
        gap: 1.5rem;
      }
      #skills {
        grid-template-columns: repeat(auto-fit,minmax(120px,1fr));
      }
    }

  </style>
</head>
<body>

  <nav>
    <div class="logo"></div>
    <ul>
      <li><a href="#about" class="active">درباره من</a></li>
      <li><a href="#skills">مهارت‌ها</a></li>
      <li><a href="#services">خدمات</a></li>
      <li><a href="#projects">نمونه‌کارها</a></li>
      <li><a href="#testimonials">نظرات</a></li>
      
      <li><button id="toggleMode" title="تغییر تم">☀️</button></li>
    </ul>
  </nav>

  <header>
    <h1></h1>
    <p>برنامه‌نویس حرفه‌ای پایتون، اکسل و توسعه‌دهنده فرم‌های لاگین امن</p>
    <button class="btn" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">ارتباط با من</button>
    <div id="liveTime" style="margin-top: 0.8rem; font-weight: 700; font-size: 1rem; color: var(--clr-primary); user-select:none;"></div>
  </header>

  <div id="profile-fixed" aria-label="پروفایل ثابت">
    <img src="https://up.20script.ir/file/2320-IMG-20240919-211857-397.jpg" alt="عکس یحیی طاهری" />
    <a href="https://t.me/hesamt65" target="_blank" title="تلگرام"><i class="fab fa-telegram"></i></a>
    <a href="https://instagram.com/hesamtaheri65" target="_blank" title="اینستاگرام"><i class="fab fa-instagram"></i></a>
    <a href="mailto:mytaheri65@gmail.com" title="ایمیل"><i class="fa-solid fa-envelope"></i></a>
  </div>

  <section id="about" tabindex="0" aria-label="درباره من">
    <img src="https://up.20script.ir/file/2320-IMG-20240919-211857-397.jpg" alt="یحیی طاهری" loading="lazy" />
    <div>
      <h2>درباره من</h2>
      <p>من یحیی طاهری هستم، برنامه‌نویس حرفه‌ای با تخصص در پایتون، طراحی فرم‌های لاگین امن و اتوماسیون اکسل. بیش از ۵ سال تجربه توسعه نرم‌افزار و پروژه‌های سفارشی دارم. هدفم ارائه راهکارهای دقیق، امن و کاملاً سفارشی برای کسب‌وکارهاست.</p>
      <p>علاقه‌مند به یادگیری مستمر و بکارگیری تکنولوژی‌های نوین برای خلق تجربه کاربری بهتر.</p>
    </div>
  </section>

  <section id="skills" aria-label="مهارت‌ها">
    <h2>مهارت‌ها</h2>
    <div class="skill-circle" data-skill="پایتون" data-percent="90" tabindex="0" aria-describedby="skill-python-desc">
      <svg width="140" height="140" viewBox="0 0 120 120" >
        <circle class="skill-bg" cx="60" cy="60" r="54"></circle>
        <circle class="skill-progress" cx="60" cy="60" r="54"></circle>
      </svg>
      <div class="skill-text">90%</div>
      <div class="skill-name" id="skill-python-desc">پایتون</div>
    </div>
    <div class="skill-circle" data-skill="اتوماسیون اکسل" data-percent="85" tabindex="0" aria-describedby="skill-excel-desc">
      <svg width="140" height="140" viewBox="0 0 120 120" >
        <circle class="skill-bg" cx="60" cy="60" r="54"></circle>
        <circle class="skill-progress" cx="60" cy="60" r="54"></circle>
      </svg>
      <div class="skill-text">85%</div>
      <div class="skill-name" id="skill-excel-desc">اتوماسیون و VBA اکسل</div>
    </div>
    <div class="skill-circle" data-skill="فرم‌های لاگین امن" data-percent="80" tabindex="0" aria-describedby="skill-login-desc">
      <svg width="140" height="140" viewBox="0 0 120 120" >
        <circle class="skill-bg" cx="60" cy="60" r="54"></circle>
        <circle class="skill-progress" cx="60" cy="60" r="54"></circle>
      </svg>
      <div class="skill-text">80%</div>
      <div class="skill-name" id="skill-login-desc">طراحی فرم‌های لاگین امن</div>
    </div>
  </section>

  <section id="services" aria-label="خدمات من">
    <h2>خدمات من</h2>
    <div class="service-card" tabindex="0" aria-label="توسعه نرم‌افزار با پایتون">
      <i class="fab fa-python"></i>
      <h3>توسعه نرم‌افزار با پایتون</h3>
      <p>برنامه‌نویسی دقیق، سریع و حرفه‌ای با پایتون برای انواع پروژه‌ها.</p>
    </div>
    <div class="service-card" tabindex="0" aria-label="اتوماسیون اکسل و VBA">
      <i class="fa-solid fa-file-excel"></i>
      <h3>اتوماسیون اکسل و VBA</h3>
      <p>طراحی فرم‌ها، گزارش‌ها و اتوماسیون دقیق در اکسل برای بهبود کارایی.</p>
    </div>
    <div class="service-card" tabindex="0" aria-label="فرم‌های لاگین امن">
      <i class="fa-solid fa-lock"></i>
      <h3>فرم‌های لاگین امن</h3>
      <p>ایجاد فرم‌های لاگین با امنیت بالا و قابلیت توسعه آسان.</p>
    </div>
  </section>

  <section id="projects" aria-label="نمونه‌کارها">
    <h2>نمونه‌کارها</h2>
    <div class="swiper mySwiper" aria-live="polite" aria-atomic="true">
      <div class="swiper-wrapper">
        <article class="swiper-slide" tabindex="0" aria-label="اتوماسیون حرفه‌ای اکسل">
          <img src="https://up.20script.ir/file/2320-photo-۲۰۲.jpg" alt="پروژه اتوماسیون اکسل" loading="lazy" class="project-img" />
          <h3 class="project-title">اتوماسیون حرفه‌ای اکسل</h3>
          <p class="project-desc">اتوماسیون وظایف روزانه و گزارش‌گیری سریع با پایتون و VBA.</p>
          <div class="project-tags" aria-label="برچسب‌ها">
            <span class="tag">Python</span>
            <span class="tag">Excel</span>
            <span class="tag">VBA</span>
          </div>
        </article>

        <article class="swiper-slide" tabindex="0" aria-label="فرم لاگین امن">
          <img src="https://via.placeholder.com/400x250?text=Secure+Login" alt="سیستم لاگین امن" loading="lazy" class="project-img" />
          <h3 class="project-title">فرم لاگین امن</h3>
          <p class="project-desc">سیستم احراز هویت و کنترل دسترسی کاربران با امنیت بالا.</p>
          <div class="project-tags" aria-label="برچسب‌ها">
            <span class="tag">Security</span>
            <span class="tag">Auth</span>
            <span class="tag">Forms</span>
          </div>
        </article>
      </div>

      <div class="swiper-pagination" tabindex="0" role="region" aria-label="صفحه‌بندی نمونه‌کارها"></div>
      <div class="swiper-button-prev" tabindex="0" role="button" aria-label="اسلاید قبلی"></div>
      <div class="swiper-button-next" tabindex="0" role="button" aria-label="اسلاید بعدی"></div>
    </div>
  </section>

  <section id="testimonials" aria-label="نظرات مشتریان">
    <h2>نظرات مشتریان</h2>
    <div class="swiper mySwiperTestimonials" aria-live="polite" aria-atomic="true">
      <div class="swiper-wrapper">
        <blockquote class="swiper-slide testimonial-slide" tabindex="0" aria-label="نظر مشتری مهدی رضایی">
          <p>"یحیی با دقت و سرعت بالا پروژه من را انجام داد، بسیار حرفه‌ای و قابل اعتماد."</p>
          <cite class="testimonial-author">– مهدی رضایی</cite>
        </blockquote>
        <blockquote class="swiper-slide testimonial-slide" tabindex="0" aria-label="نظر مشتری سارا احمدی">
          <p>"کدنویسی‌های دقیق و پشتیبانی عالی از یحیی باعث شد پروژه ما با کیفیت باشد."</p>
          <cite class="testimonial-author">– سارا احمدی</cite>
        </blockquote>
      </div>
      <div class="swiper-pagination" tabindex="0" role="region" aria-label="صفحه‌بندی نظرات"></div>
    </div>
  </section>


  <button id="backToTop" title="بازگشت به بالا" aria-label="بازگشت به بالای صفحه">
    <i class="fa-solid fa-chevron-up"></i>
  </button>

  <!-- Swiper JS -->
  <script src="https://cdn.jsdelivr.net/npm/swiper@9/swiper-bundle.min.js"></script>

  <script>
    // انیمیشن نمودار مهارت‌ها
    const circles = document.querySelectorAll('.skill-progress');
    const skillCircles = document.querySelectorAll('.skill-circle');

    skillCircles.forEach((circleWrapper) => {
      const circle = circleWrapper.querySelector('.skill-progress');
      const percent = parseInt(circleWrapper.getAttribute('data-percent'));
      const circumference = 2 * Math.PI * 54;
      const offset = circumference - (percent / 100) * circumference;
      circle.style.strokeDashoffset = offset;
    });

    // تایم زنده هدر
    const liveTime = document.getElementById('liveTime');
    function updateTime() {
      const now = new Date();
      const options = {weekday: 'long', year: 'numeric', month: 'long', day: 'numeric', hour:'2-digit', minute:'2-digit', second:'2-digit'};
      const persianDate = now.toLocaleDateString('fa-IR', options);
      liveTime.textContent = persianDate;
    }
    setInterval(updateTime, 1000);
    updateTime();

    // اسکرول smooth و فعال کردن لینک ناوبری
    const navLinks = document.querySelectorAll('nav ul li a');
    navLinks.forEach(link => {
      link.addEventListener('click', e => {
        navLinks.forEach(l => l.classList.remove('active'));
        e.target.classList.add('active');
      });
    });

    // Lazy Load تصاویر خودکار (با loading="lazy" در img هست)

    // Swiper نمونه کارها
    const swiperProjects = new Swiper('.mySwiper', {
      slidesPerView: 1,
      spaceBetween: 20,
      loop: true,
      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev',
      },
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },
      autoplay: {
        delay: 7000,
        disableOnInteraction: false,
      },
    });

    // Swiper نظرات
    const swiperTestimonials = new Swiper('.mySwiperTestimonials', {
      slidesPerView: 1,
      loop: true,
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
      },
      autoplay: {
        delay: 8000,
        disableOnInteraction: false,
      },
    });


    // دکمه بازگشت به بالا
    const backToTop = document.getElementById('backToTop');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 250) backToTop.style.display = 'block';
      else backToTop.style.display = 'none';
    });
    backToTop.addEventListener('click', () => {
      window.scrollTo({top: 0, behavior: 'smooth'});
    });

    // تغییر تم تیره و روشن
    const toggleMode = document.getElementById('toggleMode');
    toggleMode.addEventListener('click', () => {
      document.body.classList.toggle('light');
      if(document.body.classList.contains('light')){
        toggleMode.textContent = '🌙';
      } else {
        toggleMode.textContent = '☀️';
      }
    });

  </script>
</body>
</html>
