---
layout: default
title: Walmart+ Exclusive Deals
---

<style>
  :root {
    --walmart-blue: #0071ce;
    --walmart-dark: #1a365d;
    --walmart-yellow: #ffc220;
  }
  body {
    font-family: 'Inter', sans-serif;
    margin: 0;
    padding: 0;
    color: #2d3748;
    line-height: 1.5;
  }
  .header {
    background: white;
    padding: 24px 0;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
    position: sticky;
    top: 0;
    z-index: 10;
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
    box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.03);
    border: 1px solid rgba(0, 0, 0, 0.05);
    position: relative;
    overflow: hidden;
  }
  .offer-badge {
    position: absolute;
    top: 20px;
    right: -30px;
    background: var(--walmart-yellow);
    color: var(--walmart-dark);
    padding: 4px 32px;
    transform: rotate(45deg);
    font-weight: 700;
    font-size: 12px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  .cta-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    background: var(--walmart-blue);
    color: white !important;
    padding: 16px 32px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    font-size: 16px;
    transition: all 0.2s;
    box-shadow: 0 4px 6px rgba(0, 113, 206, 0.2);
    margin-top: 16px;
  }
  .cta-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 12px rgba(0, 113, 206, 0.25);
    background: #0065b8;
  }
  @media (max-width: 640px) {
    .container {
      padding: 24px 16px;
    }
    .offer-card {
      padding: 24px 16px;
    }
  }
</style>

<header class="header">
  <div style="max-width: 1200px; margin: 0 auto; padding: 0 24px;">
    <div style="display: flex; align-items: center; gap: 12px;">
      <div style="width: 32px; height: 32px; background: #0071ce; border-radius: 8px; display: flex; align-items: center; justify-content: center;">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="white">
          <path d="M12,2L1,12H4V22H20V12H23M11,15V18H13V15M15,15V18H17V15M7,15V18H9V15Z"/>
        </svg>
      </div>
      <span style="font-weight: 600; color: #1a365d;">Walmart Cashback</span>
    </div>
  </div>
</header>

<div class="container">
  <div class="offer-card">
    <div class="offer-badge">EXCLUSIVE</div>
    <h1 style="color: var(--walmart-dark); margin-top: 0; font-size: 28px;">15% Grocery Cashback</h1>
    <p style="color: #4a5568;">Verified Walmart+ members receive automatic cashback on every order for 30 days.</p>
    
    <div style="margin: 24px 0;">
      <div style="display: flex; align-items: center; gap: 8px; margin-bottom: 12px;">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="#0071ce">
          <path d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L6,13L7.41,11.59L11,14.17L16.59,8.58L18,9L11,16.5Z"/>
        </svg>
        <span>Works with pickup & delivery</span>
      </div>
      <div style="display: flex; align-items: center; gap: 8px; margin-bottom: 12px;">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="#0071ce">
          <path d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L6,13L7.41,11.59L11,14.17L16.59,8.58L18,9L11,16.5Z"/>
        </svg>
        <span>No minimum purchase required</span>
      </div>
      <div style="display: flex; align-items: center; gap: 8px;">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="#0071ce">
          <path d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L6,13L7.41,11.59L11,14.17L16.59,8.58L18,9L11,16.5Z"/>
        </svg>
        <span>Cash paid via PayPal or gift cards</span>
      </div>
    </div>
    
    <a href="/walmart-cashback/verify" class="cta-button">
      Verify My Membership
      <svg width="16" height="16" viewBox="0 0 24 24" fill="white" style="margin-left: 8px;">
        <path d="M4,11V13H16L10.5,18.5L11.92,19.92L19.84,12L11.92,4.08L10.5,5.5L16,11H4Z"/>
      </svg>
    </a>
  </div>

  <div style="display: flex; justify-content: center; gap: 32px; margin: 48px 0; flex-wrap: wrap;">
    <div style="display: flex; align-items: center; gap: 8px; font-size: 14px; color: #4a5568;">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="#0071ce">
        <path d="M12,1L3,5V11C3,16.55 6.84,21.74 12,23C17.16,21.74 21,16.55 21,11V5L12,1M10,17L6,13L7.41,11.59L10,14.17L16.59,7.58L18,9L10,17Z"/>
      </svg>
      <span>256-bit Encryption</span>
    </div>
    <div style="display: flex; align-items: center; gap: 8px; font-size: 14px; color: #4a5568;">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="#0071ce">
        <path d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L6,13L7.41,11.59L11,14.17L16.59,8.58L18,9L11,16.5Z"/>
      </svg>
      <span>Guaranteed Payouts</span>
    </div>
  </div>
</div>

<script>
// Show success message if coming from CPAGrip
if(new URLSearchParams(window.location.search).has('verified')) {
  document.body.innerHTML = `
    <div style="text-align:center; padding:40px; font-family: 'Inter', sans-serif;">
      <svg width="60" height="60" viewBox="0 0 24 24" fill="#38a169" style="margin-bottom: 20px;">
        <path d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M11,16.5L6,13L7.41,11.59L11,14.17L16.59,8.58L18,9L11,16.5Z"/>
      </svg>
      <h2 style="color: #1a365d; margin: 0 0 16px;">Verification Complete!</h2>
      <p style="color: #4a5568; max-width: 400px; margin: 0 auto 24px;">
        Your 15% cashback is now active. Returns will be processed within 24 hours.
      </p>
      <a href="/walmart-cashback" style="display: inline-block; background: #0071ce; color: white; padding: 12px 24px; border-radius: 6px; text-decoration: none; font-weight: 500;">
        Continue to Offers
      </a>
    </div>
  `;
}
</script>
