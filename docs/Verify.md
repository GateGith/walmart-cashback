---
title: "Walmart Cashback Verification"
layout: default
css: "/assets/css/style.css"
---

<div class="verification-container">
  <div class="walmart-header">
    <img src="https://i.imgur.com/JfAnW4C.png" alt="Walmart Logo" width="120">
    <h1>Walmart Grocery Cashback</h1>
    <p class="verified-badge">✔ Official Partner Program</p>
  </div>

  <div class="verification-message">
    <div class="loader"></div>
    <p class="redirect-text">Verifying your location for cashback eligibility...</p>
    
    <div class="offer-details">
      <h3>12% Cashback Activated</h3>
      <p>Free Delivery on Orders $35+</p>
    </div>
  </div>

  <div class="user-comments">
    <h4>Recent Cashback Success Stories:</h4>
    <div class="comment">
      <strong>SarahK</strong>
      <p>"Received $8.42 back on my first order!"</p>
    </div>
  </div>

  <div class="cta-footer">
    <a href="https://www.walmart.com/grocery" class="cta-button">Continue to Walmart Grocery</a>
    <p class="small-text">Redirecting automatically in <span id="countdown">5</span> seconds...</p>
  </div>
</div>

<script>
// 5-second countdown
let seconds = 5;
const countdown = setInterval(() => {
  document.getElementById('countdown').textContent = --seconds;
  if(seconds <= 0) {
    clearInterval(countdown);
    window.location.href = "https://www.walmart.com/grocery";
  }
}, 1000);
</script>

<style>
.verification-container {
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
}
.loader {
  border: 5px solid #f3f3f3;
  border-top: 5px solid #0071cc;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  animation: spin 1s linear infinite;
  margin: 20px auto;
}
@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}
.cta-button {
  background: #ffc220;
  color: #000;
  padding: 12px 24px;
  border-radius: 50px;
  font-weight: bold;
}
</style>
