---
layout: default
title: Home
---

<style>
  body {
    background: #0f172a;
    color: #e2e8f0;
  }

  .hero {
    background: linear-gradient(135deg, #0f172a, #1e293b);
    color: white;
    border-radius: 20px;
    padding: 70px 40px;
    text-align: center;
    margin-bottom: 40px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.4);
  }

  .hero h1 {
    font-size: 40px;
    margin-bottom: 10px;
    color: #38bdf8;
  }

  .hero p {
    font-size: 18px;
    color: #94a3b8;
    margin-bottom: 5px;
  }

  .info-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 25px;
  }

  .card {
    background: #1e293b;
    border-radius: 15px;
    padding: 25px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.3);
    border-left: 4px solid #38bdf8;
    text-align: center;
    transition: 0.3s;
  }

  .card:hover {
    transform: translateY(-8px);
    box-shadow: 0 10px 30px rgba(0,0,0,0.5);
  }

  .card .icon {
    font-size: 32px;
    margin-bottom: 10px;
  }

  .card h3 {
    font-size: 14px;
    color: #94a3b8;
    margin-bottom: 5px;
  }

  .card p {
    font-size: 16px;
    font-weight: bold;
    color: #e2e8f0;
  }
</style>

<div class="hero">
  <h1>Ahmad Saeed</h1>
  <p>Computer Engineering Student</p>
  <p>University of Engineering & Technology (UET) Faisalabad</p>
</div>

<div class="info-cards">
  <div class="card">
    <div class="icon">🎓</div>
    <h3>Degree</h3>
    <p>BS Computer Engineering</p>
  </div>

  <div class="card">
    <div class="icon">🏛️</div>
    <h3>University</h3>
    <p>UET Faisalabad</p>
  </div>

  <div class="card">
    <div class="icon">🏙️</div>
    <h3>Home City</h3>
    <p>Sargodha</p>
  </div>

  <div class="card">
    <div class="icon">📅</div>
    <h3>Semester</h3>
    <p>2nd Semester</p>
  </div>

  <div class="card">
    <div class="icon">💻</div>
    <h3>Skills</h3>
    <p>Python, C#, Database, GitHub</p>
  </div>
</div>
