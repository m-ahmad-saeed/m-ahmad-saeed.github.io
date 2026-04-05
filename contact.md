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
    fill: #00f5d4;
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
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M20 4H4C2.9 4 2 4.9 2 6v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/>
      </svg>
    </div>
    <h3>Email</h3>
    <p><a href="mailto:ahmadsaeed3029@gmail.com">ahmadsaeed3029@gmail.com</a></p>
  </div>

  <!-- GitHub -->
  <div class="contact-card">
    <div class="icon">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M12 0C5.37 0 0 5.37 0 12c0 5.3 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 
        0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61-.546-1.385-1.335-1.755-1.335-1.755
        -1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 
        3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 
        0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 
        3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 
        2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 
        1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 
        2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 21.795 
        24 17.295 24 12c0-6.63-5.37-12-12-12z"/>
      </svg>
    </div>
    <h3>GitHub</h3>
    <p><a href="https://github.com/m-ahmad-saeedz" target="_blank">m-ahmad-saeedz</a></p>
  </div>

  <!-- WhatsApp -->
  <div class="contact-card">
    <div class="icon">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15
        -.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475
        -.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52
        .149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207
        -.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372
        -.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 
        2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 
        1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413
        -.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l
        -.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 
        4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 
        6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 
        0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654
        a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 
        11.821 0 00-3.48-8.413z"/>
      </svg>
    </div>
    <h3>WhatsApp</h3>
    <p><a href="https://wa.me/923148664274" target="_blank">+92 3148664274</a></p>
  </div>

  <!-- University -->
  <div class="contact-card">
    <div class="icon">
      <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M12 3L1 9l11 6 9-4.91V17h2V9L12 3zM5 13.18v4L12 21l7-3.82v-4L12 17l-7-3.82z"/>
      </svg>
    </div>
    <h3>University</h3>
    <p>UET Faisalabad</p>
  </div>

</div>
