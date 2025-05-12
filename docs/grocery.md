---
title: "Walmart Grocery Cashback"
layout: default
css: "/assets/css/style.css"
---

# 🛒 Walmart Grocery Cashback  
**Verified Working {{ site.time | date: "%B %Y" }}**  

<div class="offer-banner">
<h3>12% CASHBACK</h3>
<p>Free Delivery on Orders $35+</p>
</div>

[🛒 CLAIM NOW](/verify){: .cta-button }

<div class="deal-countdown" style="color:#e31837;">
⏳ <strong>Time left:</strong> <span id="countdown">00:24:00</span>
</div>

### 🔥 Today's Hot Deals
- 🥑 Organic Produce: **+5% Bonus**  
- 🥛 Dairy Essentials: **8% Back**  
- 🍞 Bakery Items: **10% Cashback**  

<script>
// 24-Minute Countdown (Starting Red)
(function() {
  const endTime = new Date();
  endTime.setMinutes(endTime.getMinutes() + 24);
  
  function updateTimer() {
    const now = new Date();
    const diff = endTime - now;
    
    if (diff <= 0) {
      document.getElementById("countdown").textContent = "00:00:00";
      return;
    }
    
    const mins = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
    const secs = Math.floor((diff % (1000 * 60)) / 1000);
    
    document.getElementById("countdown").textContent = 
      `00:${mins.toString().padStart(2,'0')}:${secs.toString().padStart(2,'0')}`;
  }
  
  setInterval(updateTimer, 1000);
  updateTimer();
})();
</script>

<style>
:root {
  --walmart-blue: #0071cc;
  --walmart-yellow: #ffc220;
  --dark-blue: #004f9a;
}

.cta-button {
  display: block;
  background: var(--walmart-yellow);
  color: #000;
  text-align: center;
  padding: 12px 24px;
  border-radius: 50px;
  font-weight: bold;
  text-decoration: none;
  margin: 25px auto;
  width: 80%;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  transition: all 0.3s;
}

.cta-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 12px rgba(0,0,0,0.15);
}

.offer-banner {
  background: linear-gradient(135deg, var(--walmart-blue), var(--dark-blue));
  color: white;
  padding: 15px;
  border-radius: 8px;
  text-align: center;
  margin: 20px 0;
}

.deal-countdown {
  background: #fff8e1;
  padding: 12px;
  border-left: 4px solid var(--walmart-yellow);
  margin: 15px 0;
  text-align: center;
  font-weight: bold;
}
</style>
<script>
document.addEventListener('DOMContentLoaded', function() {
  fetch('https://ipapi.co/json/')
    .then(response => response.json())
    .then(data => {
      if(data.country === 'US') {
        document.querySelectorAll('.us-deal').forEach(el => {
          el.style.display = 'block';
        });
        document.body.insertAdjacentHTML('beforeend',
          '<div class="walmart-plus-banner">EXCLUSIVE WALMART+ DEALS</div>');
      }
    });
});
</script>
