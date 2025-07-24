+++
title = "Kontakt"
+++

<div class="centered-content single-flex">
<div class="kontakt-info" style="text-align: center; width: 100%;">
  <h2>Kontaktiere uns</h2>
  <p class="f6 lh-copy">
    Besuche uns auch auf: 
    <a href="https://www.instagram.com/strays_in_need_serbia/" class="link light-blue hover-white">
      <u>Instagram</u>
    </a>
  </p>
</div>

<form action="https://formsubmit.co/straysinneedserbia@gmail.com" method="POST" class="kontakt-formular" onsubmit="return showPopup();" style="margin: 0 auto; max-width: 800px;">
  <input type="text" name="_honey" style="display:none">
  <input type="hidden" name="_captcha" value="false">

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
<option value="Mitglied werden">Mitglied werden</option>
<option value="Patenschaften">Patenschaften</option>
<option value="Freiwilligenarbeit">Freiwilligenarbeit</option>
<option value="Pflegestelle">Pflegestelle</option>
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
</script>
</div>
