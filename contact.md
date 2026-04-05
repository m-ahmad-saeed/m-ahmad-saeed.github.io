---
layout: default
title: Contact
---

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
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
    color: #00f5d4;
    margin-bottom: 10px;
  }
  .contact-header p {
    font-size: 16px;
    color: #cbd5e1;
  }
  .contact-cards {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 25px;
  }
  @media (max-width: 768px) {
    .contact-cards {
      grid-template-columns: 1fr;
    }
  }
  .contact-card {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(12px);
    border-radius: 15px;
    padding: 30px;
    text-align: center;
    border: 1px solid rgba(255,255,255,0.1);
    transition: 0.3s;
  }
  .contact-card:hover {
    transform: scale(1.05);
    background: rgba(255, 255, 255, 0.15);
  }
  .contact-card .icon {
    margin-bottom: 15px;
  }
  .contact-card .icon i {
    font-size: 45px;
    color: #00f5d4 !important;
  }
  .contact-card h3 {
    font-size: 14px;
    color: #94a3b8;
    margin-bottom: 8px;
  }
  .contact-card p {
    font-size: 15px;
    font-weight: bold;
    color: #ffffff;
  }
  .contact-card a {
    color: #00f5d4;
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
    <div class="icon">
      <i class="fas fa-envelope"></i>
    </div>
    <h3>Email</h3>
    <p><a href="mailto:ahmadsaeed3029@gmail.com">ahmadsaeed3029@gmail.com</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">
      <i class="fab fa-github"></i>
    </div>
    <h3>GitHub</h3>
    <p><a href="https://github.com/m-ahmad-saeedz" target="_blank">m-ahmad-saeedz</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">
      <i class="fab fa-whatsapp"></i>
    </div>
    <h3>WhatsApp</h3>
    <p><a href="https://wa.me/923148664274" target="_blank">+92 3148664274</a></p>
  </div>

  <div class="contact-card">
    <div class="icon">
      <i class="fas fa-graduation-cap"></i>
    </div>
    <h3>University</h3>
    <p>UET Faisalabad</p>
  </div>

</div>
