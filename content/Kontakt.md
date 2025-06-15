+++
title = "Kontakt"
+++

<h2>Kontaktiere uns</h2>
<p class="f6 lh-copy">
  Besuche uns auch auf: 
  <a href="https://www.instagram.com/strays_in_need_serbia/" class="link light-blue hover-white">
    <u>Instagram</u>
  </a>
</p>

<style>
  form.kontakt-formular {
    max-width: 500px;
    padding: 1rem;
    border-radius: 8px;
    background: #f8f8f8;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  }
  form.kontakt-formular input, 
  form.kontakt-formular textarea,
  form.kontakt-formular select {
    width: 100%;
    padding: 0.6rem;
    margin-bottom: 1rem;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  .counter {
    font-size: 0.8rem;
    color: #555;
    text-align: right;
  }
  .popup {
    display: none;
    background-color: #dff0d8;
    padding: 1rem;
    border: 1px solid #3c763d;
    color: #3c763d;
    margin-top: 1rem;
    border-radius: 4px;
  }
</style>

<form action="https://formsubmit.co/straysinneedserbia@gmail.com" method="POST" class="kontakt-formular" onsubmit="return showPopup();">
  
  <!-- Anti-Spam -->
  <input type="text" name="_honey" style="display:none">
  <input type="hidden" name="_captcha" value="false">

  <!-- Optional redirect after submit -->
  <!-- <input type="hidden" name="_next" value="https://deine-seite.de/danke/"> -->

<label>Name:<span style="color: red;"> \*</span>
<input type="text" name="name" required placeholder="Max Mustermann" />
</label>

<label>Email:<span style="color: red;"> \*</span>
<input type="email" name="email" required placeholder="max@example.com" />
</label>

<label>Betreff:
<select name="betreff">
<option value="Allgemeine Anfrage">Allgemeine Anfrage</option>
<option value="Spende">Spende</option>
<option value="Adoption">Adoption</option>
<option value="Sonstiges">Sonstiges</option>
</select>
</label>

<label>Nachricht:<span style="color: red;"> \*</span>
<textarea name="nachricht" id="nachricht" rows="5" maxlength="600" required placeholder="Deine Nachricht an uns..."></textarea>
<div class="counter"><span id="zeichen">0</span>/600 Zeichen</div>
</label>

<button type="submit">Senden</button>

</form>

<div class="popup" id="popup">
  ✅ Danke für deine Nachricht! Wir melden uns bald bei dir.
</div>

<script>
  // Zeichenzähler
  const textarea = document.getElementById('nachricht');
  const counter = document.getElementById('zeichen');
  textarea.addEventListener('input', () => {
    counter.textContent = textarea.value.length;
  });

  // Popup anzeigen nach Absenden
  function showPopup() {
    const popup = document.getElementById('popup');
    popup.style.display = 'block';
    setTimeout(() => {
      popup.style.display = 'none';
    }, 4000);
    return true; // Weiterleiten erlauben
  }
</script>
