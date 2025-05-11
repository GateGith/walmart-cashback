---
title: "Grocery Cashback Deals"
layout: default
css: "/assets/css/style.css"
---

# 🛒 Weekly Grocery Specials  
**12% Cashback** • **Free Delivery** on $35+  

[🛒 CLAIM NOW](https://playabledownload.com/1802469?tid=GROCERY&utm_source=github&utm_medium=cashback){: .btn .btn-green }  

<div class="alert">
⚠️ **HURRY!** Double cashback for first 50 users today  
</div>

## Today's Hot Deals  
- 🥑 Organic Avocados: **+5% bonus**  
- 🥛 Great Value Milk: **8% back**  
- 🍞 Bread & Bakery: **10% cashback**  

<div class="deal-countdown">
⏰ Deal ends in <span id="countdown">23:59:59</span>
</div>

<script>
// Main Timer
function updateTimer() {
  const now = new Date();
  const end = new Date();
  end.setHours(23,59,59); // Today at midnight
  
  const diff = end - now;
  const hours = Math.floor(diff / (1000 * 60 * 60));
  const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
  const seconds = Math.floor((diff % (1000 * 60)) / 1000);
  
  document.getElementById("countdown").textContent = 
    `${hours.toString().padStart(2,'0')}:${minutes.toString().padStart(2,'0')}:${seconds.toString().padStart(2,'0')}`;
}
setInterval(updateTimer, 1000);
updateTimer();

// Urgency Effects
const timer = document.getElementById("countdown");
setInterval(() => {
  const timeParts = timer.textContent.split(':');
  if (parseInt(timeParts[0]) < 1) {
    timer.style.color = "#ff0000";
    timer.style.animation = 'blink 1s infinite';
  }
}, 1000);
</script>

<style>
@keyframes blink { 50% { opacity: 0.5; } }
</style>
