---
layout: default
title: Contact
---
<style>
  body {
    background: linear-gradient(135deg, #141e30, #243b55);
    color: #ffffff;
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
  .contact-card .icon svg {
    width: 45px;
    height: 45px;
    fill: #00f5d4 !important;
  }
  .contact-card .icon svg path {
    fill: #00f5d4 !important;
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

  <!-- Email -->
  <div class="contact-card">
    <div class="icon">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" style="fill:#00f5d4; width:45px; height:45px;">
        <path fill="#00f5d4" d="M20 4H4C2.9 4 2 4.9 2 6v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
      </svg>
    </div>
    <h3>Email</h3>
    <p><a href="mailto:ahmadsaeed3029@gmail.com">ahmadsaeed3029@gmail.com</a></p>
  </div>

  <!-- GitHub -->
  <div class="contact-card">
    <div class="icon">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" style="fill:#00f5d4; width:45px; height:45px;">
        <path fill="#00f5d4" d="M12 0C5.37 0 0
