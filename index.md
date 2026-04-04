---
layout: default
title: Home
---

<style>
  body {
    background: linear-gradient(135deg, #141e30, #243b55);
    color: #ffffff;
    font-family: Arial, sans-serif;
  }

  .hero {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(10px);
    border-radius: 20px;
    padding: 70px 40px;
    text-align: center;
    margin-bottom: 40px;
    border: 1px solid rgba(255,255,255,0.1);
  }

  .hero h1 {
    font-size: 42px;
    margin-bottom: 10px;
    color: #00f5d4;
  }

  .hero p {
    font-size: 18px;
    color: #d1d5db;
  }

  /* 2x2 grid for cards */
  .info-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* 2 columns */
    gap: 25px;
  }

  /* Mobile: 1 column */
  @media (max-width: 768px) {
    .info-cards {
      grid-template-columns: 1fr;
    }
  }

  .card {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(12px);
    border-radius: 15px;
    padding: 25px;
    text-align: center;
    border: 1px solid rgba(255,255,255,0.1);
    transition: 0.3s;
  }

  .card:hover {
    transform: scale(1.05);
    background: rgba(255, 255, 255, 0.15);
  }

  .card .icon {
    font-size: 30px;
    margin-bottom: 10px;
  }

  .card h3 {
    font-size: 14px;
    color: #cbd5e1;
    margin-bottom: 5px;
  }

  .card p {
    font-size: 16px;
    font-weight: bold;
    color: #ffffff;
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
</div>
