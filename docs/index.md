---
redirect_to: /grocery
---

<!-- Optional tracking snippet -->
<script>
// Basic visit tracking
if(window.location.search.includes('?t=')) {
  localStorage.setItem('last_visit', new Date().toISOString());
}

// Fallback redirect in case Jekyll doesn't process the front matter
setTimeout(function() {
  window.location.href = '/walmart-cashback/grocery';
}, 1000);
</script>

<!-- Simple loading message -->
<div style="text-align: center; margin-top: 50px;">
  <h2>Loading Walmart Cashback Deals...</h2>
  <p>If not redirected automatically, <a href="/walmart-cashback/grocery">click here</a></p>
</div>
