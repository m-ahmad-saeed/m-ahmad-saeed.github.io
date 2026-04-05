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
    <p>My journey started from a small village where education was not easy. Traveling daily to the city for college was difficult, but I stayed strong and focused on my goals.</p>

    <h3>2. Preparing for UET</h3>
    <p>I worked hard for the UET test, practiced regularly, and improved my concepts step by step.</p>

    <h3>3. Achieving My Goal</h3>
    <p>I passed the test and got admission in Computer Engineering. It was a proud moment for me and my family.</p>
  </div>
</div>

<!-- SEM 1 -->
<div id="sem1" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>

  <div class="journey-grid">
    <div class="journey-btn" onclick="showPage('a1')">Article 1</div>
    <div class="journey-btn" onclick="showPage('a2')">Article 2</div>
    <div class="journey-btn" onclick="showPage('a3')">Article 3</div>
  </div>
</div>

<!-- ARTICLE 1 -->
<div id="a1" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 1: My First Semester Journey</h1>

<h3>1. A Difficult Start in a New Place</h3>
<p>I came from another city, and starting my first semester was not easy. My first day at university was very difficult because it was my first experience living in a hostel. I missed my home, my family, and my comfortable life. The hostel environment was not good, food was not tasty, and I had to stay in a big hall with many students.</p>

<h3>2. Facing Hostel Life and Starting Studies</h3>
<p>The next day, classes started. Everything was new and challenging. It was difficult to manage studies and hostel life together, but slowly I adjusted and started understanding the system.</p>

<h3>3. Staying Strong</h3>
<p>Despite all difficulties, I stayed strong. These challenges made me independent and helped me grow.</p>

</div>
</div>

<!-- ARTICLE 2 -->
<div id="a2" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 2: First Semester Exams</h1>

<h3>1. Hard Work</h3>
<p>I decided to study hard and focus on concepts because university study is different.</p>

<h3>2. Understanding System</h3>
<p>The paper system was difficult at first, but I improved with practice and effort.</p>

<h3>3. Mid Success</h3>
<p>I passed my mid exams with good marks which increased my confidence.</p>

</div>
</div>

<!-- ARTICLE 3 -->
<div id="a3" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 3: Mid to Final Success</h1>

<h3>1. Study Improvement</h3>
<p>I improved my study routine and focused more on understanding.</p>

<h3>2. Friends</h3>
<p>We studied together, helped each other, and enjoyed outings.</p>

<h3>3. Final Achievement</h3>
<p>I passed finals with good marks and felt proud.</p>

</div>
</div>

<!-- SEM 2 -->
<div id="sem2" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>

  <div class="journey-grid">
    <div class="journey-btn" onclick="showPage('a4')">Article 4</div>
    <div class="journey-btn" onclick="showPage('a5')">Article 5</div>
    <div class="journey-btn" onclick="showPage('a6')">Article 6</div>
    <div class="journey-btn" onclick="showPage('a7')">Article 7</div>
  </div>
</div>

<!-- ARTICLE 4 -->
<div id="a4" class="page">
<div class="back-btn" onclick="showPage('sem2')">← Back</div>
<div class="article-body">

<h1>Article 4: Second Semester Start</h1>

<h3>1. New Beginning</h3>
<p>After vacation, I returned with confidence and a positive mindset.</p>

<h3>2. Learning from Mistakes</h3>
<p>I improved my habits and decided not to repeat past mistakes.</p>

<h3>3. Responsibility</h3>
<p>I understood the value of money and became more responsible.</p>

</div>
</div>

<!-- ARTICLE 5 -->
<div id="a5" class="page">
<div class="back-btn" onclick="showPage('sem2')">← Back</div>
<div class="article-body">

<h1>Article 5: Summer Challenges</h1>

<h3>1. Heat</h3>
<p>Summer made hostel life very difficult.</p>

<h3>2. Problems</h3>
<p>Fans were not working and mosquitoes disturbed us at night.</p>

<h3>3. Strength</h3>
<p>We stayed strong despite all problems.</p>

</div>
</div>

<!-- ARTICLE 6 -->
<div id="a6" class="page">
<div class="back-btn" onclick="showPage('sem2')">← Back</div>
<div class="article-body">

<h1>Article 6: Ramadan Experience</h1>

<h3>1. Religion</h3>
<p>We focused on Namaz and Quran.</p>

<h3>2. Iftar Issues</h3>
<p>Iftar was not good and sometimes not enough.</p>

<h3>3. Patience</h3>
<p>This time taught us patience and gratitude.</p>

</div>
</div>

<!-- ARTICLE 7 -->
<div id="a7" class="page">
<div class="back-btn" onclick="showPage('sem2')">← Back</div>
<div class="article-body">

<h1>Article 7: Online Classes and Eid</h1>

<h3>1. Online Classes</h3>
<p>We attended online classes but faced internet issues.</p>

<h3>2. Difficulty</h3>
<p>Understanding lectures was difficult due to technical problems.</p>

<h3>3. Eid</h3>
<p>We enjoyed Eid and then returned to university.</p>

</div>
</div>

<script>
function showPage(id){
 document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
 document.getElementById(id).classList.add('active');
}
</script>
