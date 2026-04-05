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
    padding: 20px;
    border-radius: 15px;
    cursor: pointer;
    transition: 0.3s;
    text-align:center;
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

<!-- MAIN PAGE -->
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

<!-- ADMISSION -->
<div id="admission" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>
  <div class="article-body">
    <h1>From Village Challenges to Computer Engineering Dreams</h1>

    <h3>1. Overcoming Early Academic Struggles</h3>
    <p>My journey started from a small village where education was not easy. Traveling daily to city for college was difficult, but I stayed strong.</p>

    <h3>2. Preparing for UET</h3>
    <p>I worked hard for UET test, practiced daily and improved my concepts.</p>

    <h3>3. Achieving My Goal</h3>
    <p>I passed the test and got admission in Computer Engineering. It was a proud moment for me.</p>
  </div>
</div>

<!-- SEM 1 LIST -->
<div id="sem1" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>

  <div class="journey-grid">
    <div class="journey-btn" onclick="showPage('a1')">Article 1</div>
    <div class="journey-btn" onclick="showPage('a2')">Article 2</div>
    <div class="journey-btn" onclick="showPage('a3')">Article 3</div>
    <div class="journey-btn" onclick="showPage('a4')">Article 4</div>
    <div class="journey-btn" onclick="showPage('a5')">Article 5</div>
    <div class="journey-btn" onclick="showPage('a6')">Article 6</div>
    <div class="journey-btn" onclick="showPage('a7')">Article 7</div>
  </div>
</div>

<!-- ARTICLE 1 -->
<div id="a1" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 1: My First Semester Journey</h1>

<h3>1. A Difficult Start</h3>
<p>I came from another city and faced many problems in hostel. Food was not good and hall was crowded.</p>

<h3>2. Adjusting Life</h3>
<p>Classes started and I slowly adjusted with study and hostel life.</p>

<h3>3. Staying Strong</h3>
<p>I stayed strong and continued my journey.</p>

</div>
</div>

<!-- ARTICLE 2 -->
<div id="a2" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 2: First Semester Exams</h1>

<h3>1. Hard Work</h3>
<p>I decided to study hard and understand concepts.</p>

<h3>2. System Difficulty</h3>
<p>University system was difficult but I improved.</p>

<h3>3. Mid Success</h3>
<p>I passed mid exams with good marks.</p>

</div>
</div>

<!-- ARTICLE 3 -->
<div id="a3" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 3: Mid to Final</h1>

<h3>1. Study Improvement</h3>
<p>I improved study habits.</p>

<h3>2. Friends</h3>
<p>We studied together and helped each other.</p>

<h3>3. Final Success</h3>
<p>I passed finals with good marks.</p>

</div>
</div>

<!-- ARTICLE 4 -->
<div id="a4" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 4: Second Semester Start</h1>

<h3>1. Confidence</h3>
<p>I returned with confidence.</p>

<h3>2. Learning</h3>
<p>I improved mistakes.</p>

<h3>3. Responsibility</h3>
<p>I understood value of money.</p>

</div>
</div>

<!-- ARTICLE 5 -->
<div id="a5" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 5: Summer Problems</h1>

<h3>1. Heat</h3>
<p>Weather was very hot.</p>

<h3>2. Problems</h3>
<p>No fans, mosquitoes, no sleep.</p>

<h3>3. Strength</h3>
<p>We stayed strong.</p>

</div>
</div>

<!-- ARTICLE 6 -->
<div id="a6" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 6: Ramadan</h1>

<h3>1. Religion</h3>
<p>Focused on Namaz and Quran.</p>

<h3>2. Iftar Issue</h3>
<p>Iftar was not good.</p>

<h3>3. Patience</h3>
<p>Learned patience.</p>

</div>
</div>

<!-- ARTICLE 7 -->
<div id="a7" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 7: Online & Eid</h1>

<h3>1. Online Classes</h3>
<p>Internet issues created problems.</p>

<h3>2. Difficulty</h3>
<p>Hard to understand lectures.</p>

<h3>3. Eid</h3>
<p>Enjoyed Eid and returned to uni.</p>

</div>
</div>

<!-- SEM 2 -->
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
