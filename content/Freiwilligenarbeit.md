+++
title = "Kontakt"
+++

<h2>Kontaktiere uns</h2>

<form name="kontakt" method="POST" data-netlify="true" netlify-honeypot="bot-field">
  <!-- Anti-Spam -->
  <input type="hidden" name="form-name" value="kontakt" />
  <p style="display:none">
    <label>Don’t fill this out: <input name="bot-field" /></label>
  </p>

  <p>
    <label>Name:<br />
      <input type="text" name="name" required />
    </label>
  </p>

  <p>
    <label>Email:<br />
      <input type="email" name="email" required />
    </label>
  </p>

  <p>
    <label>Nachricht:<br />
      <textarea name="nachricht" rows="5" required></textarea>
    </label>
  </p>

  <p>
    <button type="submit">Senden</button>
  </p>
</form>
