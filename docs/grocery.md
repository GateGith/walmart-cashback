---
layout: default
title: Walmart Grocery Cashback
---

<div style="max-width:600px;margin:0 auto;padding:20px">
  <h1>🛒 Get 15% Cashback on Groceries</h1>
  
  <div style="border:2px solid #0071ce;border-radius:10px;padding:25px;margin:30px 0">
    <h3>Limited-Time Offer</h3>
    <p>Exclusive to new Walmart+ members</p>
    <a href="/walmart-cashback/verify" 
       style="display:block;
              background:#0071ce;
              color:white;
              padding:15px;
              border-radius:25px;
              text-decoration:none;
              font-weight:bold;
              margin-top:20px">
      VERIFY ELIGIBILITY ➔
    </a>
  </div>
</div>
<script>
// Show confirmation if coming from CPAGrip
if(new URLSearchParams(window.location.search).has('verified')) {
  document.body.innerHTML = `
    <div style="text-align:center; padding:40px; font-family:Arial">
      <h2 style="color:#0071ce;">✅ Verification Successful!</h2>
      <p>Your Walmart+ cashback is now active.</p>
      <a href="/walmart-cashback" style="color:#0071ce;">← Back to Offers</a>
    </div>
  `;
}
</script>
