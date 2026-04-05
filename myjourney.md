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

  /* === CLICKABLE BUTTON CARD === */
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

  /* === DETAIL PANEL === */
  .detail-panel {
    display: none;
    background: rgba(255, 255, 255, 0.06);
    border-radius: 15px;
    padding: 30px;
    border: 1px solid rgba(0, 245, 212, 0.2);
    margin-top: -10px;
    animation: fadeIn 0.3s ease;
  }
  .detail-panel.open {
    display: block;
  }
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .detail-panel ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .detail-panel ul li {
    font-size: 14px;
    color: #cbd5e1;
    padding: 8px 0;
    border-bottom: 1px solid rgba(255,255,255,0.05);
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .detail-panel ul li:last-child {
    border-bottom: none;
  }
  .detail-panel ul li i {
    color: #00f5d4;
    font-size: 14px;
    min-width: 16px;
    text-align: center;
  }
  .section-title {
    font-size: 13px;
    color: #00f5d4;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin: 15px 0 8px 0;
  }
  .section-title:first-child {
    margin-top: 0;
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
    <div class="detail-panel" id="admission">
      <div class="section-title">Details</div>
      <ul>
        <li><i class="fas fa-university"></i> University of Engineering & Technology, Faisalabad</li>
        <li><i class="fas fa-laptop"></i> Program: BS Computer Science</li>
        <li><i class="fas fa-check-circle"></i> Successfully cleared merit-based admission</li>
      </ul>
    </div>
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
    <div class="detail-panel" id="sem1">
      <div class="section-title">Subjects</div>
      <ul>
        <li><i class="fas fa-code"></i> Introduction to Computing</li>
        <li><i class="fas fa-calculator"></i> Calculus & Analytical Geometry</li>
        <li><i class="fas fa-atom"></i> Applied Physics</li>
        <li><i class="fas fa-pen"></i> English Composition & Comprehension</li>
        <li><i class="fas fa-star-and-crescent"></i> Islamic Studies / Ethics</li>
      </ul>
      <div class="section-title">Highlights</div>
      <ul>
        <li><i class="fas fa-star"></i> Got familiar with university environment</li>
        <li><i class="fas fa-star"></i> Learned basics of programming</li>
      </ul>
    </div>
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
    <div class="detail-panel" id="sem2">
      <div class="section-title">Subjects</div>
      <ul>
        <li><i class="fas fa-code"></i> Object Oriented Programming (OOP)</li>
        <li><i class="fas fa-calculator"></i> Linear Algebra</li>
        <li><i class="fas fa-microchip"></i> Digital Logic Design</li>
        <li><i class="fas fa-pen"></i> Communication Skills</li>
        <li><i class="fas fa-flag"></i> Pakistan Studies</li>
      </ul>
      <div class="section-title">Highlights</div>
      <ul>
        <li><i class="fas fa-star"></i> Learned OOP concepts in C++</li>
        <li><i class="fas fa-star"></i> Built first small projects</li>
      </ul>
    </div>
  </div>

</div>

<script>
  function togglePanel(id, btn) {
    const panel = document.getElementById(id);
    const isOpen = panel.classList.contains('open');

    // Close all panels
    document.querySelectorAll('.detail-panel').forEach(p => p.classList.remove('open'));
    document.querySelectorAll('.journey-btn').forEach(b => b.classList.remove('active'));

    // Open clicked one if it was closed
    if (!isOpen) {
      panel.classList.add('open');
      btn.classList.add('active');
    }
  }
</script>
