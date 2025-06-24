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

---

## 💖 Support QuadPixel

<div class="notice--info">
  Help us keep making awesome indie chaos. Choose a quick tip or set a custom amount!
</div>

<div class="page__content" style="border: 1px solid var(--border-color); padding: 1rem; border-radius: 0.5rem; background: var(--background-color);">

<div style="display: flex; flex-wrap: wrap; gap: 1rem; align-items: center;">

  <!-- Quick Buttons -->
  <div style="display: flex; gap: 0.5rem;">
    <button type="button" onclick="setAmount(10)" class="btn btn--primary">₹10</button>
    <button type="button" onclick="setAmount(20)" class="btn btn--primary">₹20</button>
    <button type="button" onclick="setAmount(50)" class="btn btn--primary">₹50</button>
  </div>

  <!-- Slider -->
  <div style="display: flex; align-items: center; gap: 0.5rem;">
    <input type="range" id="customAmount" min="1" max="200" value="30" style="width: 150px;">
    <span id="amountLabel" style="font-weight: bold;">₹30</span>
  </div>

  <!-- Donate Button -->
  <a id="upiLink"
     href="upi://pay?pa=aatikshnew@okicici&pn=AATIKSH%20SINHA%20MINOR&cu=INR&am=30&tn=Support%20QuadPixel"
     class="btn btn--success">
    Donate ₹30
  </a>

</div>
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
