<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Car Detailing Ganterschwil</title>
<style>
    /* --- Reset & základní styl --- */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Georgia', serif; }
    body { background-color: #f5e6d3; color: #3a2c21; line-height: 1.6; padding: 20px; }

    h1, h2, h3 { font-family: 'Georgia', serif; margin-bottom: 10px; }
    h1 { font-size: 2.5em; color: #b08644; text-align: center; margin-bottom: 20px; }
    h2 { color: #3a2c21; margin-top: 20px; }
    h3 { color: #3a2c21; margin-top: 15px; }

    p, li { font-size: 1.1em; margin-bottom: 10px; }

    /* --- Layout --- */
    .container { max-width: 800px; margin: 0 auto; background: #f5e6d3; padding: 30px; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1);}
    ul { list-style: none; padding-left: 0; }
    ul li::before { content: "• "; color: #b08644; font-weight: bold; }

    /* --- Tlačítka a odkazy --- */
    a, button { display: inline-block; background-color: #b08644; color: #fff; text-decoration: none; padding: 10px 20px; border-radius: 5px; transition: 0.3s; border: none; cursor: pointer; }
    a:hover, button:hover { background-color: #8a6239; }

    /* --- Formulář --- */
    form { margin-top: 20px; }
    input, textarea { width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #3a2c21; border-radius: 5px; font-family: 'Georgia', serif; }
    textarea { resize: vertical; }
    .success { color: green; margin-top: 10px; }

    /* --- Animace --- */
    .star { color: #b08644; transition: transform 0.3s; }
    .star:hover { transform: scale(1.3); }

    /* --- Ikony (ASCII/emoji jako ilustrace) --- */
    .icon { font-size: 2em; margin-right: 10px; vertical-align: middle; }
</style>
</head>
<body>

<div class="container">
    <h1>✨ CAR DETAILING GANTERSCHWIL ✨</h1>
    <p style="text-align:center; font-style: italic;">Professionelle Autopflege – Ihr Fahrzeug in Bestform</p>

    <h2>Unsere Leistungen</h2>
    <ul>
        <li>Handwäsche & gründliche Innenreinigung</li>
        <li>Lackkorrektur & Wachsversiegelung</li>
        <li>Keramikbeschichtungen & Premium-Schutz</li>
        <li>Scheinwerfer-Aufbereitung & Geruchsbeseitigung</li>
    </ul>

    <p>📍 Ganterschwil | Mobil & Werkstatt-Service<br>
       📲 WhatsApp / Tel.: 0783324498<br>
       📷 Instagram: <a href="https://instagram.com/cardetailingganterschwil" target="_blank">@cardetailingganterschwil</a></p>

    <h2>Pakete im Überblick</h2>
    <ul>
        <li>Basic (CHF 90–120): Handwäsche, Staubsaugen, Fenster</li>
        <li>Standard (CHF 220–280): Innen & Außen gründlich, Pflege von Kunststoffen</li>
        <li>Premium (CHF 400–650): Lackkorrektur, Keramik-Schutz, Lederpflege</li>
        <li>Luxury (CHF 950–1’500+): Mehrstufige Politur, 2–5 Jahre Keramik, Komplettaufbereitung</li>
    </ul>

    <h2>Unsere Slogans</h2>
    <ul>
        <li>„Glanz, der bleibt.“ <span class="star">⭐</span></li>
        <li>„Ihr Auto verdient Premium-Pflege.“ <span class="star">⭐</span></li>
        <li>„Detailgenauigkeit bis ins kleinste Teil.“ <span class="star">⭐</span></li>
        <li>„Weil jedes Fahrzeug einzigartig ist.“ <span class="star">⭐</span></li>
        <li>„Von matt zu brillant – Car Detailing Ganterschwil.“ <span class="star">⭐</span></li>
    </ul>

    <h2>Kontaktieren Sie uns</h2>
    <form id="contactForm">
        <input type="text" name="name" placeholder="Ihr Name" required>
        <input type="email" name="email" placeholder="Ihre E-Mail" required>
        <textarea name="message" rows="5" placeholder="Ihre Nachricht" required></textarea>
        <button type="submit">Nachricht senden</button>
        <p class="success" id="successMsg" style="display:none;">Vielen Dank! Ihre Nachricht wurde gesendet.</p>
    </form>
</div>

<script>
document.getElementById('contactForm').addEventListener('submit', function(e){
    e.preventDefault();
    const form = e.target;
    const data = new FormData(form);
    const email = "cardetailing-ganterschwil@gmail.com"; // Změň na svůj e-mail
    const subject = "Neue Nachricht von Car Detailing Webseite";
    const body = `Name: ${data.get('name')}\nEmail: ${data.get('email')}\nNachricht:\n${data.get('message')}`;
    
    window.location.href = `mailto:${email}?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
    document.getElementById('successMsg').style.display = "block";
    form.reset();
});
</script>

</body>
</html>
