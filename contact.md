---
layout: default
title: Contact
---

<style>
  body {
    background: #0f172a;
    color: #e2e8f0;
    font-family: Arial, sans-serif;
  }

  .contact-header {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(10px);
    border-radius: 20px;
    padding: 50px;
    margin-bottom: 30px;
    text-align: center;
    border: 1px solid rgba(255,255,255,0.1);
  }

  .contact-header h1 {
    font-size: 36px;
    color: #38bdf8;
    margin-bottom: 10px;
  }

  .contact-header p {
    font-size: 16px;
    color: #94a3b8;
  }

  .contact-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* 2 columns */
    gap: 25px;
    margin-top: 20px;
  }

  @media (max-width: 768px) {
    .contact-cards {
      grid-template-columns: 1fr; /* mobile: single column */
    }
  }

  .contact-card {
    background: rgba(255,255,255,0.08);
    backdrop-filter: blur(12px);
    border-radius: 15px;
    padding: 30px;
    text-align: center;
    border: 1px solid rgba(255,255,255,0.1);
    transition: 0.3s;
  }

  .contact-card:hover {
    transform: scale(1.05);
    background: rgba(255,255,255,0.15);
  }

  .contact-card .icon {
    font-size: 40px;
    margin-bottom: 15px;
  }

  .contact-card h3 {
    font-size: 14px;
    color: #cbd5e1;
    margin-bottom: 8px;
  }

  .contact-card p {
    font-size: 15px;
    font-weight: bold;
    color: #ffffff;
  }

  .contact-card a {
    color: #38bdf8;
    text-decoration: none;
  }

  .contact-card a:hover {
    text-decoration: underline;
  }
</style>

<div class="contact-header">
  <h1>Contact Me</h1>
  <p>Feel free to reach out anytime!</p>
</div>

<div class="contact-cards">
  <div class="contact-card">
    <div class="icon">📧</div>
    <h3>Email</h3>
    <p><a href="mailto:ahmedsaeed3029@gmail.com">ahmedsaeed3029@gmail.com</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">💬</div>
    <h3>WhatsApp</h3>
    <p><a href="https://wa.me/923148664274" target="_blank">03148664274</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">🐙</div>
    <h3>GitHub</h3>
    <p><a href="https://github.com/ahmedsaeed3029" target="_blank">ahmedsaeed3029</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">🎓</div>
    <h3>University</h3>
    <p>UET Faisalabad</p>
  </div>
</div>
