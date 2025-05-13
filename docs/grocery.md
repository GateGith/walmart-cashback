---
layout: default
title: Walmart+ Cashback Deals
---

<style>
  :root {
    --primary: #0071ce;
    --primary-dark: #1a365d;
    --accent: #ffc220;
    --gray-100: #f7fafc;
    --gray-800: #2d3748;
  }
  
  body {
    font-family: 'Inter', system-ui, sans-serif;
    margin: 0;
    padding: 0;
    color: var(--gray-800);
    line-height: 1.5;
  }
  
  .header {
    background: white;
    padding: 24px 0;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
    position: relative;
    z-index: 10;
  }
  
  .header-content {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 24px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .logo {
    display: flex;
    align-items: center;
    gap: 12px;
    font-weight: 600;
    color: var(--primary-dark);
    text-decoration: none;
  }
  
  .logo-svg {
    width: 32px;
    height: 32px;
    background: var(--primary);
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .logo-svg svg {
    width: 20px;
    height: 20px;
    fill: white;
  }
  
  .container {
    max-width: 800px;
    margin: 0 auto;
    padding: 40px 24px;
  }
  
  .offer-card {
    background: white;
    border-radius: 12px;
    padding: 32px;
    margin-bottom: 32px;
    box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.03), 0 4px 6px -2px rgba(0, 0, 0, 0.02);
    border: 1px solid rgba(0, 0, 0, 0.05);
    position: relative;
    overflow: hidden;
  }
  
  .offer-badge {
    position: absolute;
    top: 20px;
    right: -30px;
    background: var(--accent);
    color: var(--primary-dark);
    padding: 4px 32px;
    transform: rotate(45deg);
    font-weight: 700;
    font-size: 12px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .offer-title {
    color: var(--primary-dark);
    margin-top: 0;
    font-size: 24px;
    font-weight: 700;
  }
  
  .offer-features {
    margin: 24px 0;
    padding: 0;
    list-style: none;
  }
  
  .offer-features li {
    padding: 8px 0;
    position: relative;
    padding-left: 28px;
  }
  
  .offer-features li:before {
    content: "";
    position: absolute;
    left: 0;
    top: 12px;
    width: 16px;
    height: 16px;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%230071ce'%3E%3Cpath d='M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L18,9.5L16.59,8.09L11,13.67L7.91,10.59L6.5,12L11,16.5Z'/%3E%3C/svg%3E");
    background-size: contain;
  }
  
  .cta-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    background: var(--primary);
    color: white !important;
    padding: 16px 32px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    font-size: 16px;
    transition: all 0.2s;
    border: none;
    cursor: pointer;
    box-shadow: 0 4px 6px rgba(0, 113, 206, 0.2);
    margin-top: 8px;
  }
  
  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 12px rgba(0, 113, 206, 0.25);
    background: #0065b8;
  }
  
  .cta-button svg {
    margin-left: 8px;
    width: 16px;
    height: 16px;
  }
  
  .trust-badges {
    display: flex;
    justify-content: center;
    gap: 32px;
    margin: 48px 0;
    flex-wrap: wrap;
  }
  
  .trust-badge {
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 14px;
    color: #4a5568;
  }
  
  .trust-badge svg {
    flex-shrink: 0;
    width: 20px;
    height: 20px;
    fill: var(--primary);
  }
  
  @media (max-width: 640px) {
    .container {
      padding: 24px 16px;
    }
    
    .offer-card {
      padding: 24px 16px;
    }
    
    .trust-badges {
      gap: 24px;
      margin: 32px 0;
    }
  }
</style>

<header class="header">
  <div class="header-content">
    <a href="/walmart-cashback" class="logo">
      <div class="logo-svg">
        <svg viewBox="0 0 24 24">
          <path d="M12,2L1,12H4V22H20V12H23M11,15V18H13V15M15,15V18H17V15M7,15V18H9V15Z"/>
        </svg>
      </div>
      <span>Walmart Cashback</span>
    </a>
  </div>
</header>

<div class="container">
  <div class="offer-card">
    <div class="offer-badge">EXCLUSIVE</div>
    <h2 class="offer-title">15% Grocery Cashback</h2>
    <p style="color: #4a5568;">Verified Walmart+ members receive automatic cashback on every grocery order for 30 days.</p>
    
    <ul class="offer-features">
      <li>Works with pickup & delivery orders</li>
      <li>Stacks with existing promotions</li>
      <li>No minimum purchase required</li>
      <li>Cash paid via PayPal or gift cards</li>
    </ul>
    
    <a href="/walmart-cashback/verify" class="cta-button">
      Claim My Cashback
      <svg viewBox="0 0 24 24">
        <path d="M4,11V13H16L10.5,18.5L11.92,19.92L19.84,12L11.92,4.08L10.5,5.5L16,11H4Z"/>
      </svg>
    </a>
  </div>

  <div class="trust-badges">
    <div class="trust-badge">
      <svg viewBox="0 0 24 24">
        <path d="M12,1L3,5V11C3,16.55 6.84,21.74 12,23C17.16,21.74 21,16.55 21,11V5L12,1M12,11.99H19C18.47,16.11 15.72,19.78 12,20.93V12H5V6.3L12,3.19V11.99Z"/>
      </svg>
      <span>256-bit SSL Encryption</span>
    </div>
    <div class="trust-badge">
      <svg viewBox="0 0 24 24">
        <path d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L18,9.5L16.59,8.09L11,13.67L7.91,10.59L6.5,12L11,16.5Z"/>
      </svg>
      <span>Guaranteed Payouts</span>
    </div>
    <div class="trust-badge">
      <svg viewBox="0 0 24 24">
        <path d="M12,3C16.97,3 21,7.03 21,12C21,16.97 16.97,21 12,21C7.03,21 3,16.97 3,12C3,7.03 7.03,3 12,3M12,5C8.14,5 5,8.14 5,12C5,15.86 8.14,19 12,19C15.86,19 19,15.86 19,12C19,8.14 15.86,5 12,5M13,17H11V15H13V17M13,13H11V7H13V13Z"/>
      </svg>
      <span>24/7 Support</span>
    </div>
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
