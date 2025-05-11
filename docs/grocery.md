<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Walmart Grocery Cashback</title>
    <style>
        :root {
            --walmart-blue: #0071ce;
            --walmart-yellow: #ffc220;
            --dark-blue: #004f9a;
            --white: #ffffff;
            --black: #000000;
            --green: #00a862;
            --red: #e31837;
        }
        
        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f7f7f7;
            color: #333;
            line-height: 1.6;
        }
        
        .header {
            text-align: center;
            margin-bottom: 25px;
        }
        
        h1 {
            color: var(--walmart-blue);
            font-size: 28px;
            margin-bottom: 5px;
        }
        
        h2 {
            color: var(--dark-blue);
            font-size: 22px;
            margin-top: 0;
            font-weight: 500;
        }
        
        .offer-banner {
            background: linear-gradient(135deg, var(--walmart-blue), var(--dark-blue));
            color: white;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            margin: 20px 0;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        
        .offer-banner h3 {
            margin: 0;
            font-size: 24px;
        }
        
        .offer-banner p {
            margin: 10px 0 0;
            font-size: 16px;
        }
        
        .cta-button {
            display: block;
            background-color: var(--walmart-yellow);
            color: var(--black);
            text-align: center;
            padding: 12px;
            border-radius: 50px;
            font-weight: bold;
            text-decoration: none;
            font-size: 18px;
            margin: 25px auto;
            width: 80%;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            transition: transform 0.2s;
        }
        
        .cta-button:hover {
            transform: translateY(-2px);
            background-color: #ffd24d;
        }
        
        .deal-item {
            background-color: var(--white);
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            display: flex;
            align-items: center;
        }
        
        .deal-item input[type="checkbox"] {
            margin-right: 15px;
            transform: scale(1.3);
        }
        
        .deal-text {
            flex: 1;
        }
        
        .deal-text span {
            font-weight: bold;
            color: var(--green);
        }
        
        .countdown {
            background-color: var(--red);
            color: white;
            padding: 10px 15px;
            border-radius: 8px;
            text-align: center;
            margin: 30px 0;
            font-size: 18px;
        }
        
        .countdown-timer {
            font-size: 24px;
            font-weight: bold;
            margin-top: 5px;
            letter-spacing: 1px;
        }
        
        .checked {
            opacity: 0.7;
            position: relative;
        }
        
        .checked:after {
            content: "✓ CLAIMED";
            position: absolute;
            right: 15px;
            background-color: var(--green);
            color: white;
            padding: 3px 8px;
            border-radius: 12px;
            font-size: 12px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>walmart-cashback</h1>
        <h2>Weekly Grocery Specials</h2>
    </div>
    
    <div class="offer-banner">
        <h3>12% Cashback</h3>
        <p>Free Delivery on $35+</p>
    </div>
    
    <a href="#" class="cta-button">CLAIM NOW</a>
    
    <div style="text-align: center; margin: 20px 0; font-weight: bold; color: var(--red);">
        <strong>HURRY!</strong> Double cashback for first 50 users today
    </div>
    
    <h3 style="color: var(--dark-blue); border-bottom: 2px solid var(--walmart-yellow); padding-bottom: 5px;">Today's Hot Deals</h3>
    
    <div class="deal-item">
        <input type="checkbox" id="avocados">
        <label for="avocados" class="deal-text">Organic Avocados: <span>+5% bonus</span></label>
    </div>
    
    <div class="deal-item">
        <input type="checkbox" id="milk">
        <label for="milk" class="deal-text">Great Value Milk: <span>8% back</span></label>
    </div>
    
    <div class="deal-item checked">
        <input type="checkbox" id="bread" checked disabled>
        <label for="bread" class="deal-text">Bread & Bakery: <span>10% cashback</span></label>
    </div>
    
    <div class="countdown">
        <div>Deal ends in <span id="countdown-days">72</span>h <span id="countdown-hours">0</span>m <span id="countdown-minutes">0</span>s</div>
        <div class="countdown-timer" id="live-countdown">24:00:00</div>
    </div>

    <script>
        // Countdown Timer
        function updateCountdown() {
            const now = new Date();
            const endTime = new Date(now);
            endTime.setHours(now.getHours() + 24); // 24-hour countdown
            
            const diff = endTime - now;
            
            if (diff <= 0) {
                document.getElementById('live-countdown').textContent = "EXPIRED";
                return;
            }
            
            const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((diff % (1000 * 60)) / 1000);
            
            document.getElementById('live-countdown').textContent = 
                `${hours.toString().padStart(2, '0')}:${minutes.toString().padStart(2, '0')}:${seconds.toString().padStart(2, '0')}`;
        }
        
        // Initial call and set interval
        updateCountdown();
        setInterval(updateCountdown, 1000);
        
        // Deal checkboxes functionality
        document.querySelectorAll('.deal-item input[type="checkbox"]').forEach(checkbox => {
            checkbox.addEventListener('change', function() {
                if (this.checked) {
                    this.parentElement.classList.add('checked');
                    this.disabled = true;
                }
            });
        });
    </script>
</body>
</html>
