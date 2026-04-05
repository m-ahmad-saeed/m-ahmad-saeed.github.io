---
layout: default
title: My Journey
---
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
  .journey-header {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(10px);
    border-radius: 20px;
    padding: 50px;
    margin-bottom: 40px;
    text-align: center;
    border: 1px solid rgba(255,255,255,0.1);
  }
  .journey-header h1 { font-size: 36px; color: #00f5d4; margin-bottom: 10px; }
  .journey-header p { font-size: 16px; color: #cbd5e1; }

  .journey-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
  }

  .journey-btn {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(12px);
    border-radius: 15px;
    padding: 30px;
    border: 1px solid rgba(255,255,255,0.1);
    cursor: pointer;
    transition: 0.3s;
    text-align: left;
    width: 100%;
    text-decoration: none;
    display: block;
  }
  .journey-btn:hover {
    transform: translateY(-5px);
    background: rgba(255, 255, 255, 0.14);
    border-color: #00f5d4;
    text-decoration: none;
  }
  .icon-circle {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    background: rgba(0, 245, 212, 0.12);
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 12px;
  }
  .icon-circle i { font-size: 26px; color: #00f5d4; }
  .btn-label {
    font-size: 12px;
    color: #00f5d4;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 4px;
  }
  .btn-title { font-size: 18px; color: #ffffff; font-weight: bold; }
  .btn-date { font-size: 13px; color: #94a3b8; margin-top: 6px; }
  .btn-date i { color: #00f5d4; margin-right: 4px; }

  /* === ARTICLE PAGE === */
  .page { display: none; }
  .page.active { display: block; }

  .back-btn {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    color: #00f5d4;
    font-size: 14px;
    text-decoration: none;
    margin-bottom: 30px;
    padding: 8px 16px;
    border: 1px solid rgba(0,245,212,0.3);
    border-radius: 8px;
    cursor: pointer;
    background: none;
    transition: 0.3s;
  }
  .back-btn:hover { background: rgba(0,245,212,0.1); }

  .article-header {
    background: rgba(255, 255, 255, 0.08);
    border-radius: 20px;
    padding: 40px;
    margin-bottom: 30px;
    border: 1px solid rgba(255,255,255,0.1);
    display: flex;
    align-items: center;
    gap: 20px;
  }
  .article-icon-circle {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    background: rgba(0, 245, 212, 0.12);
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
  }
  .article-icon-circle i { font-size: 30px; color: #00f5d4; }
  .article-header h1 { font-size: 28px; color: #ffffff; margin: 0 0 5px 0; }
  .article-header p { color: #94a3b8; font-size: 14px; margin: 0; }

  .article-body {
    background: rgba(255, 255, 255, 0.06);
    border-radius: 15px;
    padding: 35px;
    border: 1px solid rgba(255,255,255,0.1);
    animation: fadeIn 0.3s ease;
  }
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .article-body p { font-size: 15px; color: #cbd5e1; line-height: 1.9; margin-bottom: 15px; }
  .article-body h3 { font-size: 17px; color: #00f5d4; margin: 25px 0 10px 0; }
  .article-body ul { list-style: none; padding: 0; margin: 0 0 15px 0; }
  .article-body ul li {
    font-size: 14px;
    color: #cbd5e1;
    padding: 8px 0;
    border-bottom: 1px solid rgba(255,255,255,0.05);
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .article-body ul li:last-child { border-bottom: none; }
  .article-body ul li i { color: #00f5d4; min-width: 16px; }

  @media (max-width: 768px) {
    .journey-grid { grid-template-columns: 1fr; }
  }
</style>

<!-- ===== MAIN PAGE ===== -->
<div id="main-page" class="page active">

  <div class="journey-header">
    <h1>My Journey</h1>
    <p>My academic path at UET Faisalabad — semester by semester</p>
  </div>

  <div class="journey-grid">

    <div class="journey-btn" onclick="showPage('admission')">
      <div class="icon-circle"><i class="fas fa-flag-checkered"></i></div>
      <div class="btn-label">Starting Point</div>
      <div class="btn-title">Admission</div>
      <div class="btn-date"><i class="fas fa-calendar-alt"></i> 2023</div>
    </div>

    <div class="journey-btn" onclick="showPage('sem1')">
      <div class="icon-circle"><i class="fas fa-graduation-cap"></i></div>
      <div class="btn-label">Semester 1</div>
      <div class="btn-title">First Semester</div>
      <div class="btn-date"><i class="fas fa-calendar-alt"></i> Fall 2023</div>
    </div>

    <div class="journey-btn" onclick="showPage('sem2')">
      <div class="icon-circle"><i class="fas fa-book-open"></i></div>
      <div class="btn-label">Semester 2</div>
      <div class="btn-title">Second Semester</div>
      <div class="btn-date"><i class="fas fa-calendar-alt"></i> Spring 2024</div>
    </div>

  </div>
</div>

<!-- ===== ADMISSION PAGE ===== -->
<div id="admission" class="page">
  <button class="back-btn" onclick="showPage('main-page')">
    <i class="fas fa-arrow-left"></i> Back to My Journey
  </button>
  <div class="article-header">
    <div class="article-icon-circle"><i class="fas fa-flag-checkered"></i></div>
    <div>
      <h1>Admission — UET Faisalabad</h1>
      <p><i class="fas fa-calendar-alt"></i> 2023 &nbsp;|&nbsp; Starting Point</p>
    </div>
  </div>
  <div class="article-body">
    <!-- APNA ARTICLE YAHAN LIKHEN -->
    <p>
      It was 2023 when I got admitted to UET Faisalabad in BS Computer Science.
      Getting into UET was a dream come true for me. I worked hard in FSc and
      cleared the merit-based admission test successfully.
    </p>
    <p>
      UET Faisalabad is one of the top engineering universities in Pakistan.
      I chose Computer Science because I have always been passionate about
      technology and programming. I knew this was the right path for me.
    </p>
    <h3><i class="fas fa-list"></i> Details</h3>
    <ul>
      <li><i class="fas fa-university"></i> University of Engineering & Technology, Faisalabad</li>
      <li><i class="fas fa-laptop"></i> Program: BS Computer Science</li>
      <li><i class="fas fa-check-circle"></i> Successfully cleared merit-based admission</li>
    </ul>
  </div>
</div>

<!-- ===== SEMESTER 1 PAGE ===== -->
<div id="sem1" class="page">
  <button class="back-btn" onclick="showPage('main-page')">
    <i class="fas fa-arrow-left"></i> Back to My Journey
  </button>
  <div class="article-header">
    <div class="article-icon-circle"><i class="fas fa-graduation-cap"></i></div>
    <div>
      <h1>First Semester</h1>
      <p><i class="fas fa-calendar-alt"></i> Fall 2023 &nbsp;|&nbsp; Semester 1</p>
    </div>
  </div>
  <div class="article-body">
    <!-- APNA ARTICLE YAHAN LIKHEN -->
    <p>
      My first semester at UET Faisalabad was an incredible experience.
      Coming from school, university life was completely different.
      I had to manage my time carefully between studies and other activities.
    </p>
    <p>
      The most exciting subject was Introduction to Computing where I wrote
      my first ever program — a simple Hello World in C++!
    </p>
    <h3><i class="fas fa-book"></i> Subjects</h3>
    <ul>
      <li><i class="fas fa-code"></i> Introduction to Computing</li>
      <li><i class="fas fa-calculator"></i> Calculus & Analytical Geometry</li>
      <li><i class="fas fa-atom"></i> Applied Physics</li>
      <li><i class="fas fa-pen"></i> English Composition & Comprehension</li>
      <li><i class="fas fa-star-and-crescent"></i> Islamic Studies / Ethics</li>
    </ul>
    <h3><i class="fas fa-star"></i> Highlights</h3>
    <ul>
      <li><i class="fas fa-star"></i> Got familiar with university environment</li>
      <li><i class="fas fa-star"></i> Learned basics of programming</li>
    </ul>
  </div>
</div>

<!-- ===== SEMESTER 2 PAGE ===== -->
<div id="sem2" class="page">
  <button class="back-btn" onclick="showPage('main-page')">
    <i class="fas fa-arrow-left"></i> Back to My Journey
  </button>
  <div class="article-header">
    <div class="article-icon-circle"><i class="fas fa-book-open"></i></div>
    <div>
      <h1>Second Semester</h1>
      <p><i class="fas fa-calendar-alt"></i> Spring 2024 &nbsp;|&nbsp; Semester 2</p>
    </div>
  </div>
  <div class="article-body">
    <!-- APNA ARTICLE YAHAN LIKHEN -->
    <p>
      Second semester was more challenging and exciting than the first one.
      We dived deeper into programming with Object Oriented Programming in C++.
      I built my first small projects this semester which gave me a lot of confidence.
    </p>
    <p>
      OOP was my favorite subject. Building real projects using classes and
      objects in C++ was very satisfying!
    </p>
    <h3><i class="fas fa-book"></i> Subjects</h3>
    <ul>
      <li><i class="fas fa-code"></i> Object Oriented Programming (OOP)</li>
      <li><i class="fas fa-calculator"></i> Linear Algebra</li>
      <li><i class="fas fa-microchip"></i> Digital Logic Design</li>
      <li><i class="fas fa-pen"></i> Communication Skills</li>
      <li><i class="fas fa-flag"></i> Pakistan Studies</li>
    </ul>
    <h3><i class="fas fa-star"></i> Highlights</h3>
    <ul>
      <li><i class="fas fa-star"></i> Learned OOP concepts in C++</li>
      <li><i class="fas fa-star"></i> Built first small projects</li>
    </ul>
  </div>
</div>

<script>
  function showPage(id) {
    document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
    document.getElementById(id).classList.add('active');
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
</script>
