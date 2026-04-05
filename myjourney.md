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

<h3>1. A Difficult Start in a New Place</h3>
<p>I came from another city, and starting my first semester was not easy. My first day at university was very difficult because it was my first experience living in a hostel. I missed my home, my family, and my comfortable life. Everything felt new and uncomfortable. The hostel environment was also not good for me. The food was not tasty, and I was given a big hall where many boys were living together. There was noise and no privacy, which made it hard for me to adjust..</p>

<h3>2. Facing Hostel Life and Starting Studies</h3>
<p>The next day, we went to the university, and our classes started. This was the beginning of a new academic journey. The environment was different from college, and the level of study was more difficult. I had to manage both hostel life and studies at the same time. In the beginning, it was very hard for me, but slowly I started understanding things and adjusting to this new life..</p>

<h3>3. Staying Strong</h3>
<p>I Even though I faced many problems, I decided to stay strong. I knew that this was an important step in my life. These challenges made me more independent and responsible. Slowly, I started feeling better and became part of university life..</p>

</div>
</div>

<!-- ARTICLE 2 -->
<div id="a2" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 2: First Semester Exams</h1>

<h3>1.Making a Promise to Work Hard</h3>
<p>I When our studies started, I made a strong decision that I would study hard and become successful in life. Teachers told us that university education is conceptual, which means we must understand topics deeply instead of just memorizing them.</p>

<h3>2. Understanding the New System</h3>
<p>The paper system was completely different from what I experienced before. At first, I faced difficulty in understanding it. I felt confused and stressed, but I did not give up. I started asking questions, studying more, and improving my concepts step by step.</p>

<h3>3. Mid Success</h3>
<p>I After two months, our mid exams started. It was my first university exam, and it was difficult. However, I worked hard and gave my best. When the results came, I passed with good marks. This success increased my confidence..</p>

</div>
</div>

<!-- ARTICLE 3 -->
<div id="a3" class="page">
<div class="back-btn" onclick="showPage('sem1')">← Back</div>
<div class="article-body">

<h1>Article 3: From Midterms to Finals: Friendship, Growth, and Success</h1>

<h3>1.Improving Study Habits</h3>
<p>I After mid exams, I gained some experience about university studies. I started managing my time better and focused more on understanding concepts. I created a study routine and followed it regularly.</p>

<h3>2. Friendship and Support</h3>
<p>In the hostel, we became friends with each other. We studied together, helped each other in difficult subjects, and shared our problems. Sometimes, we also went out for outings to relax. Although the hostel food was not good, we managed everything together.</p>

<h3>3. Final Exams Achievement</h3>
<p>After two months, final exams started. They were challenging, but I was better prepared this time. I gave my best effort, and Alhamdulillah, I passed with good marks. It was a proud moment for me..</p>

</div>
</div>


</div>

<!-- SEM 2 -->
<div id="sem2" class="page">
  <div class="back-btn" onclick="showPage('main-page')">← Back</div>
  <p>Coming soon...</p>
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

<script>
function showPage(id){
 document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
 document.getElementById(id).classList.add('active');
}
</script>
