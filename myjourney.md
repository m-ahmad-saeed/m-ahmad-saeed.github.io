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

  @media (max-width: 768px) {
    .journey-grid { grid-template-columns: 1fr; }
  }
</style>

<div id="main-page" class="page active">
  <div class="journey-header">
    <h1>My Journey</h1>
    <p>My academic path — from village to university</p>
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

<div id="admission" class="page">
  <button class="back-btn" onclick="showPage('main-page')">
    <i class="fas fa-arrow-left"></i> Back to My Journey
  </button>

  <div class="article-header">
    <div class="article-icon-circle"><i class="fas fa-flag-checkered"></i></div>
    <div>
      <h1>From Village Challenges to Computer Engineering Dreams</h1>
      <p><i class="fas fa-calendar-alt"></i> 2023 &nbsp;|&nbsp; My Admission Story</p>
    </div>
  </div>

  <div class="article-body">
    <h3>1. Overcoming Early Academic Struggles</h3>
    <p>
      My educational journey has never been easy. Coming from a small village, I faced several challenges during my FSc studies. The lack of nearby educational facilities and guidance made learning difficult. Every day, traveling to the city for college was exhausting and sometimes felt impossible. Despite these difficulties, I stayed determined and focused on my goal. The competitive environment of college pushed me to work harder, improve my skills, and adapt to new challenges.
    </p>

    <h3>2. Preparing for the UET Test</h3>
    <p>
      After completing my college studies, the next big challenge was preparing for the UET entry test. I knew that getting admission in Computer Engineering would not be easy. I made a proper study plan, revised important subjects, and practiced past papers regularly. This phase was mentally tough, but it taught me discipline, time management, and consistency. My previous struggles gave me the confidence to keep moving forward.
    </p>

    <h3>3. Achieving My Goal and Looking Forward</h3>
    <p>
      Finally, I passed the UET test and secured admission in Computer Engineering. This achievement was a turning point in my life. My journey from a village to a university proved that hard work and determination can overcome any obstacle. Now, I am continuing my journey with new goals, aiming to excel in my field and inspire others from similar backgrounds to follow their dreams.
    </p>
  </div>
</div>

<div id="sem1" class="page">
  <button class="back-btn" onclick="showPage('main-page')">
    <i class="fas fa-arrow-left"></i> Back to My Journey
  </button>
  <div class="article-header">
    <div class="article-icon-circle"><i class="fas fa-graduation-cap"></i></div>
    <div>
      <h1>First Semester</h1>
    </div>
  </div>
  <div class="article-body">
    <p>Content coming soon...</p>
  </div>
</div>

<div id="sem2" class="page">
  <button class="back-btn" onclick="showPage('main-page')">
    <i class="fas fa-arrow-left"></i> Back to My Journey
  </button>
  <div class="article-header">
    <div class="article-icon-circle"><i class="fas fa-book-open"></i></div>
    <div>
      <h1>Second Semester</h1>
    </div>
  </div>
  <div class="article-body">
    <p>Content coming soon...</p>
  </div>
</div>

<script>
function showPage(id) {
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  window.scrollTo({ top: 0, behavior: 'smooth' });
}
</script>
