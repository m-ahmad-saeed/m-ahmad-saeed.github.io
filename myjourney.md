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
  }
  .journey-header h1 { color: #00f5d4; }

  .journey-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
  }

  .journey-btn {
    background: rgba(255,255,255,0.08);
    padding: 25px;
    border-radius: 15px;
    cursor: pointer;
    transition: 0.3s;
  }
  .journey-btn:hover { transform: translateY(-5px); }

  .page { display:none; }
  .page.active { display:block; }

  .back-btn { cursor:pointer; color:#00f5d4; margin-bottom:20px; }

  .article-body { padding:30px; background:rgba(255,255,255,0.05); border-radius:15px; }
  .article-body h3 { color:#00f5d4; }

  @media(max-width:768px){
    .journey-grid { grid-template-columns:1fr; }
  }
</style>

<div id="main-page" class="page active">
  <div class="journey-header">
    <h1>My Journey</h1>
  </div>

  <div class="journey-grid">
    <div class="journey-btn" onclick="showPage('admission')">Admission</div>
    <div class="journey-btn" onclick="showPage('sem1')">Semester 1</div>
    <div class="journey-btn" onclick="showPage('sem2')">Semester 2</div>
  </div>
</div>

<div id="admission" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>
  <div class="article-body">
    <h1>From Village Challenges to Computer Engineering Dreams</h1>
    <p>Your admission article here...</p>
  </div>
</div>

<!-- SEM 1 LIST -->
<div id="sem1" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>
  <div class="journey-btn" onclick="showPage('sem1-art1')">1st Article</div>
</div>

<!-- SEM 1 ARTICLE -->
<div id="sem1-art1" class="page">
  <div class="back-btn" onclick="showPage('sem1')">← Back</div>
  <div class="article-body">

<h1>My First Semester Journey: Challenges, Adjustments, and a New Beginning</h1>

<p>Starting university life is a big step, especially when you come from another city. My first semester was full of new experiences, challenges, and lessons that helped me grow stronger and more independent.</p>

<h3>A Difficult Start in a New Place</h3>
<p>My first day at university was very difficult. It was my first time living away from my home and family.</p>

<p>The hostel environment was not what I expected. The food was not good, and I had to stay in a hall with many students.</p>

<h3>Facing Challenges and Adjusting</h3>
<p>Slowly, I started adjusting. I made friends and learned patience and tolerance.</p>

<h3>The Beginning of University Life</h3>
<p>Classes started and I focused on my studies. I promised myself to never give up.</p>

  </div>
</div>

<div id="sem2" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>
  <p>Coming soon...</p>
</div>

<script>
function showPage(id){
 document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
 document.getElementById(id).classList.add('active');
}
</script>
