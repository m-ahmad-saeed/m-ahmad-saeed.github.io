---
layout: default
title: About
---

<style>
  body {
    background: linear-gradient(135deg, #0f172a, #1e3a8a);
    color: #e2e8f0;
    font-family: 'Segoe UI', sans-serif;
  }

  .about-header {
    background: rgba(15, 23, 42, 0.7);
    backdrop-filter: blur(12px);
    border-radius: 20px;
    padding: 60px;
    margin-bottom: 30px;
    text-align: center;
    border: 1px solid rgba(59,130,246,0.2);
    box-shadow: 0 0 25px rgba(59,130,246,0.2);
  }

  .about-header h1 {
    font-size: 38px;
    color: #3b82f6;
    margin-bottom: 10px;
    letter-spacing: 1px;
  }

  .about-header p {
    color: #94a3b8;
    font-size: 16px;
  }

  .about-section {
    background: rgba(15, 23, 42, 0.6);
    backdrop-filter: blur(10px);
    border-radius: 15px;
    padding: 30px;
    margin-bottom: 20px;
    border: 1px solid rgba(59,130,246,0.15);
    transition: 0.3s;
  }

  .about-section:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(59,130,246,0.2);
  }

  .about-section h2 {
    color: #60a5fa;
    font-size: 20px;
    margin-bottom: 15px;
    border-bottom: 1px solid rgba(59,130,246,0.2);
    padding-bottom: 10px;
  }

  .about-section p {
    line-height: 1.8;
    color: #cbd5f5;
    font-size: 15px;
  }

  .skills-list {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin-top: 10px;
  }

  .skill-tag {
    background: rgba(59,130,246,0.15);
    color: #60a5fa;
    padding: 6px 18px;
    border-radius: 20px;
    font-size: 13px;
    border: 1px solid #3b82f6;
    transition: 0.3s;
  }

  .skill-tag:hover {
    background: #3b82f6;
    color: white;
  }
</style>

<div class="about-header">
  <h1>About Me</h1>
  <p>Get to know me better!</p>
</div>

<div class="about-section">
  <h2>👋 Who Am I?</h2>
  <p>My name is Ahmad Saeed. I am from Sargodha and currently studying in Faisalabad. I am a Computer Engineering student at UET Faisalabad in my 2nd semester.</p>
</div>

<div class="about-section">
  <h2>🎓 Education</h2>
  <p>Currently pursuing BS Computer Engineering at University of Engineering & Technology (UET) Faisalabad.</p>
  <br>
  <p>📘 Matric — Computer Science</p>
  <p>📗 FSC — ICS (Punjab College)</p>
  <p>📙 Currently — BS Computer Engineering at UET Faisalabad</p>
</div>

<div class="about-section">
  <h2>💻 Skills</h2>
  <div class="skills-list">
    <span class="skill-tag">Python</span>
    <span class="skill-tag">C#</span>
    <span class="skill-tag">GitHub</span>
    <span class="skill-tag">Problem Solving</span>
  </div>
</div>

<div class="about-section">
  <h2>🌟 Interests</h2>
  <p>I enjoy coding, learning new technologies, and sharing my journey through my blog. I believe in continuous learning and working hard to achieve my goals.</p>
</div>
