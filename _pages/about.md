---
permalink: /about/
title: "About QuadPixel"
---

## 🧠 About QuadPixel

QuadPixel is a tiny but mighty indie game studio focused on making chaotic, weird, and wildly fun games that don’t take themselves too seriously — and neither do we.

We’re all about ideas that make people go “wait, what?” and then “okay that was actually fun.” Whether it’s a gun that shoots beach balls, faceless blobs jumping through portals, or Kartik flapping through pipes, if it makes us laugh or rage-quit, it probably belongs in a QuadPixel game.

We're not here to win GOTY. We’re here to make dumb fun — and maybe break a few rules while we’re at it.

Come play.

## 💸 Support the Goofballs!

<p>
    <!-- 💸 Floating Horizontal UPI Panel -->
<div id="upiDonatePanel" style="position: fixed; top: 80px; right: 0; z-index: 9999;
background: #f9f9f9; border: 2px solid #00a86b; border-right: none; border-radius: 10px 0 0 10px;
padding: 12px 16px; display: flex; align-items: center; gap: 12px; box-shadow: -4px 4px 10px rgba(0,0,0,0.1);
font-family: sans-serif; max-width: 100%; flex-wrap: wrap;">

<strong>💸 Tip Us:</strong>

<div id="quickAmounts" style="display:flex; gap:6px;">
  <button type="button" onclick="setAmount(10)" style="padding:6px 10px; border:none; border-radius:4px;
  background:#e0e0e0; font-weight:bold; cursor:pointer;">₹10</button>
  <button type="button" onclick="setAmount(20)" style="padding:6px 10px; border:none; border-radius:4px;
  background:#e0e0e0; font-weight:bold; cursor:pointer;">₹20</button>
  <button type="button" onclick="setAmount(50)" style="padding:6px 10px; border:none; border-radius:4px;
  background:#e0e0e0; font-weight:bold; cursor:pointer;">₹50</button>
</div>

<div style="display:flex; align-items:center; gap:6px;">
  <input type="range" id="customAmount" min="1" max="200" value="30"
  style="width: 120px;" oninput="updateAmount(this.value)">
  <span id="amountLabel">₹30</span>
</div>

<a id="upiLink" href="upi://pay?pa=aatikshnew@okicici&pn=AATIKSH%20SINHA%20MINOR&cu=INR&am=30&tn=Support%20QuadPixel"
style="background:#00a86b;color:white;padding:8px 14px;border-radius:6px;
font-weight:bold;text-decoration:none;">Donate ₹30</a>
</div>

<script>
function setAmount(amount) {
  document.getElementById('customAmount').value = amount;
  updateAmount(amount);
}

function updateAmount(value) {
  document.getElementById('amountLabel').textContent = `₹${value}`;
  const upi = `upi://pay?pa=aatikshnew@okicici&pn=AATIKSH%20SINHA%20MINOR&cu=INR&am=${value}&tn=Support%20QuadPixel`;
  document.getElementById('upiLink').href = upi;
  document.getElementById('upiLink').textContent = `Donate ₹${value}`;
}
</script>

</p>