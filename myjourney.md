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
  .timeline {
    position: relative;
    padding-left: 40px;
  }
  .timeline::before {
    content: '';
    position: absolute;
    left: 16px;
    top: 0;
    bottom: 0;
    width: 3px;
    background: linear-gradient(to bottom, #00f5d4, #0077ff);
    border-radius: 3px;
  }
  .timeline-item {
    position: relative;
    margin-bottom: 35px;
  }
  .timeline-item::before {
    content: '';
    position: absolute;
    left: -31px;
    top: 18px;
    width: 14px;
    height: 14px;
    background: #00f5d4;
    border-radius: 50%;
    border: 3px solid #0f172a;
    box-shadow: 0 0 8px #00f5d4;
  }
  .timeline-card {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(12px);
    border-radius: 15px;
    padding: 25px 30px;
    border: 1px solid rgba(255,255,255,0.1);
    transition: 0.3s;
  }
  .timeline-card:hover {
    transform: translateX(5px);
    background: rgba(255, 255, 255, 0.14);
  }
  .card-icon-block {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin-bottom: 12px;
  }
  .card-icon-block .icon-circle {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    background: rgba(0, 245, 212, 0.12);
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 10px;
  }
  .card-icon-block .icon-circle i {
    font-size: 26px;
    color: #00f5d4;
  }
  .card-icon-block .semester-label {
    font-size: 12px;
    color: #00f5d4;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  .timeline-card h2 {
    font-size: 20px;
    color: #ffffff;
    margin: 4px 0 5px 0;
  }
  .date {
    font-size: 13px;
    color: #94a3b8;
    margin-bottom: 15px;
    display: flex;
    align-items: center;
    gap: 6px;
  }
  .date i {
    color: #00f5d4;
  }
  .timeline-card ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .timeline-card ul li {
    font-size: 14px;
    color: #cbd5e1;
    padding: 6px 0;
    border-bottom: 1px solid rgba(255,255,255,0.05);
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .timeline-card ul li:last-child {
    border-bottom: none;
  }
  .timeline-card ul li i {
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
</style>

<div class="journey-header">
  <h1>My Journey</h1>
  <p>My academic path at UET Faisalabad — semester by semester</p>
</div>

<div class="timeline">

  <!-- Admission -->
  <div class="timeline-item">
    <div class="timeline-card">
      <div class="card-icon-block">
        <div class="icon-circle">
          <i class="fas fa-flag-checkered"></i>
        </div>
        <div class="semester-label">Starting Point</div>
      </div>
      <h2>Admission — UET Faisalabad</h2>
      <div class="date"><i class="fas fa-calendar-alt"></i> 2023</div>
      <ul>
        <li><i class="fas fa-university"></i> University of Engineering & Technology, Faisalabad</li>
        <li><i class="fas fa-laptop"></i> Program: BS Computer Science</li>
        <li><i class="fas fa-check-circle"></i> Successfully cleared merit-based admission</li>
      </ul>
    </div>
  </div>

  <!-- Semester 1 -->
  <div class="timeline-item">
    <div class="timeline-card">
      <div class="card-icon-block">
        <div class="icon-circle">
          <i class="fas fa-graduation-cap"></i>
        </div>
        <div class="semester-label">Semester 1</div>
      </div>
      <h2>First Semester</h2>
      <div class="date"><i class="fas fa-calendar-alt"></i> Fall 2023</div>
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

  <!-- Semester 2 -->
  <div class="timeline-item">
    <div class="timeline-card">
      <div class="card-icon-block">
        <div class="icon-circle">
          <i class="fas fa-book-open"></i>
        </div>
        <div class="semester-label">Semester 2</div>
      </div>
      <h2>Second Semester</h2>
      <div class="date"><i class="fas fa-calendar-alt"></i> Spring 2024</div>
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
