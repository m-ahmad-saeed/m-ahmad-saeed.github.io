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
  .journey-header h1 {
    font-size: 36px;
    color: #00f5d4;
    margin-bottom: 10px;
  }
  .journey-header p {
    font-size: 16px;
    color: #cbd5e1;
  }
  .journey-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 25px;
    margin-bottom: 40px;
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
  }
  .journey-btn:hover {
    transform: translateY(-5px);
    background: rgba(255, 255, 255, 0.14);
    border-color: #00f5d4;
  }
  .journey-btn.active {
    border-color: #00f5d4;
    background: rgba(0, 245, 212, 0.08);
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
  .icon-circle i {
    font-size: 26px;
    color: #00f5d4;
  }
  .btn-label {
    font-size: 12px;
    color: #00f5d4;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 4px;
  }
  .btn-title {
    font-size: 18px;
    color: #ffffff;
    font-weight: bold;
  }
  .btn-date {
    font-size: 13px;
    color: #94a3b8;
    margin-top: 6px;
  }
  .btn-date i {
    color: #00f5d4;
    margin-right: 4px;
  }
  .btn-arrow {
    float: right;
    color: #00f5d4;
    font-size: 18px;
    margin-top: -30px;
    transition: 0.3s;
  }
  .journey-btn.active .btn-arrow {
    transform: rotate(180deg);
  }

  /* === ARTICLE PANEL === */
  .article-panel {
    display: none;
    background: rgba(255, 255, 255, 0.06);
    border-radius: 15px;
    padding: 35px;
    border: 1px solid rgba(0, 245, 212, 0.2);
    margin-top: 15px;
    animation: fadeIn 0.3s ease;
    grid-column: 1 / -1;
  }
  .article-panel.open {
    display: block;
  }
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .article-panel h3 {
    font-size: 22px;
    color: #00f5d4;
    margin-bottom: 15px;
    border-bottom: 1px solid rgba(0,245,212,0.2);
    padding-bottom: 10px;
  }
  .article-panel p {
    font-size: 15px;
    color: #cbd5e1;
    line-height: 1.8;
    margin-bottom: 15px;
  }
  .article-panel h4 {
    font-size: 16px;
    color: #ffffff;
    margin: 20px 0 8px 0;
  }
  .article-panel ul {
    list-style: none;
    padding: 0;
    margin: 0 0 15px 0;
  }
  .article-panel ul li {
    font-size: 14px;
    color: #cbd5e1;
    padding: 6px 0;
    border-bottom: 1px solid rgba(255,255,255,0.05);
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .article-panel ul li:last-child {
    border-bottom: none;
  }
  .article-panel ul li i {
    color: #00f5d4;
    font-size: 14px;
    min-width: 16px;
  }
  .close-btn {
    background: rgba(0, 245, 212, 0.1);
    border: 1px solid #00f5d4;
    color: #00f5d4;
    padding: 8px 20px;
    border-radius: 8px;
    cursor: pointer;
    font-size: 13px;
    margin-top: 10px;
    transition: 0.3s;
  }
  .close-btn:hover {
    background: #00f5d4;
    color: #0f172a;
  }
</style>

<div class="journey-header">
  <h1>My Journey</h1>
  <p>My academic path at UET Faisalabad — semester by semester</p>
</div>

<div class="journey-grid">

  <!-- Admission Button -->
  <div>
    <button class="journey-btn" onclick="togglePanel('admission', this)">
      <div class="icon-circle">
        <i class="fas fa-flag-checkered"></i>
      </div>
      <div class="btn-label">Starting Point</div>
      <div class="btn-title">Admission</div>
      <div class="btn-date"><i class="fas fa-calendar-alt"></i> 2023</div>
      <i class="fas fa-chevron-down btn-arrow"></i>
    </button>
  </div>

  <!-- Semester 1 Button -->
  <div>
    <button class="journey-btn" onclick="togglePanel('sem1', this)">
      <div class="icon-circle">
        <i class="fas fa-graduation-cap"></i>
      </div>
      <div class="btn-label">Semester 1</div>
      <div class="btn-title">First Semester</div>
      <div class="btn-date"><i class="fas fa-calendar-alt"></i> Fall 2023</div>
      <i class="fas fa-chevron-down btn-arrow"></i>
    </button>
  </div>

  <!-- Semester 2 Button -->
  <div>
    <button class="journey-btn" onclick="togglePanel('sem2', this)">
      <div class="icon-circle">
        <i class="fas fa-book-open"></i>
      </div>
      <div class="btn-label">Semester 2</div>
      <div class="btn-title">Second Semester</div>
      <div class="btn-date"><i class="fas fa-calendar-alt"></i> Spring 2024</div>
      <i class="fas fa-chevron-down btn-arrow"></i>
    </button>
  </div>

  <!-- Admission Article -->
  <div class="article-panel" id="admission">
    <h3><i class="fas fa-flag-checkered"></i> &nbsp;My Admission Story</h3>
    <p>
      <!-- APNA ARTICLE YAHAN LIKHEN -->
      It was 2023 when I got admitted to UET Faisalabad in BS Computer Science. 
      Getting into UET was a dream come true for me. I worked hard in FSc and 
      cleared the merit-based admission test successfully. The day I got my 
      admission letter was one of the happiest days of my life.
    </p>
    <p>
      UET Faisalabad is one of the top engineering universities in Pakistan. 
      I chose Computer Science because I have always been passionate about 
      technology and programming. I knew this was the right path for me.
    </p>
    <button class="close-btn" onclick="togglePanel('admission', null)">
      <i class="fas fa-times"></i> Close
    </button>
  </div>

  <!-- Semester 1 Article -->
  <div class="article-panel" id="sem1">
    <h3><i class="fas fa-graduation-cap"></i> &nbsp;First Semester Experience</h3>
    <p>
      <!-- APNA ARTICLE YAHAN LIKHEN -->
      My first semester at UET Faisalabad was an incredible experience. 
      Coming from school, university life was completely different. 
      I had to manage my time carefully between studies and other activities.
    </p>
    <h4><i class="fas fa-book"></i> Subjects I Studied</h4>
    <ul>
      <li><i class="fas fa-code"></i> Introduction to Computing — Learned basics of computers and programming</li>
      <li><i class="fas fa-calculator"></i> Calculus & Analytical Geometry — Challenging but very interesting</li>
      <li><i class="fas fa-atom"></i> Applied Physics — Fun experiments in the lab</li>
      <li><i class="fas fa-pen"></i> English Composition — Improved my writing skills</li>
      <li><i class="fas fa-star-and-crescent"></i> Islamic Studies — Learned about Islamic values</li>
    </ul>
    <p>
      The most exciting subject was Introduction to Computing where I wrote 
      my first ever program. It was a simple "Hello World" in C++ but it 
      felt amazing to see it run on screen!
    </p>
    <button class="close-btn" onclick="togglePanel('sem1', null)">
      <i class="fas fa-times"></i> Close
    </button>
  </div>

  <!-- Semester 2 Article -->
  <div class="article-panel" id="sem2">
    <h3><i class="fas fa-book-open"></i> &nbsp;Second Semester Experience</h3>
    <p>
      <!-- APNA ARTICLE YAHAN LIKHEN -->
      Second semester was more challenging and exciting than the first one. 
      We dived deeper into programming with Object Oriented Programming in C++. 
      I built my first small projects this semester which gave me a lot of confidence.
    </p>
    <h4><i class="fas fa-book"></i> Subjects I Studied</h4>
    <ul>
      <li><i class="fas fa-code"></i> OOP in C++ — Learned classes, objects, inheritance</li>
      <li><i class="fas fa-calculator"></i> Linear Algebra — Matrices and vectors</li>
      <li><i class="fas fa-microchip"></i> Digital Logic Design — Gates and circuits</li>
      <li><i class="fas fa-pen"></i> Communication Skills — Presentations and speaking</li>
      <li><i class="fas fa-flag"></i> Pakistan Studies — History of Pakistan</li>
    </ul>
    <p>
      OOP was my favorite subject this semester. Building real projects using 
      classes and objects in C++ was very satisfying. I also enjoyed Digital 
      Logic Design where we learned how computers work at the hardware level.
    </p>
    <button class="close-btn" onclick="togglePanel('sem2', null)">
      <i class="fas fa-times"></i> Close
    </button>
  </div>

</div>

<script>
  function togglePanel(id, btn) {
    const panel = document.getElementById(id);
    const isOpen = panel.classList.contains('open');

    // Close all panels and buttons
    document.querySelectorAll('.article-panel').forEach(p => p.classList.remove('open'));
    document.querySelectorAll('.journey-btn').forEach(b => b.classList.remove('active'));

    // Open clicked one if it was closed
    if (!isOpen) {
      panel.classList.add('open');
      if (btn) btn.classList.add('active');
      // Scroll to article
      setTimeout(() => {
        panel.scrollIntoView({ behavior: 'smooth', block: 'start' });
      }, 100);
    }
  }
</script>
