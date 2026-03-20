<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>It Sees – Multiplayer Survival Game</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="Sees.css">

<style>
/* Cookie Banner */
#cookie-banner {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    background: #111;
    color: white;
    padding: 15px;
    text-align: center;
    z-index: 1000;
}

#cookie-banner button {
    margin-left: 10px;
    padding: 8px 14px;
    background: #4CAF50;
    border: none;
    color: white;
    cursor: pointer;
    border-radius: 4px;
}

#cookie-banner button:hover {
    background: #45a049;
}
</style>

</head>

<body>

<header>
    <h1>Seescape</h1>
    <p>
        A multiplayer survival game built around asymmetric gameplay,
        stealth, cooperation, and dynamic light-based mechanics.
    </p>
</header>

<section>
<h2>About the Game</h2>
<p>
<strong>It Sees</strong> is a multiplayer survival experience where survivors
must work together using light and strategy to evade powerful monsters.
Vision, darkness, and coordination define every match.
</p>

<div class="image-placeholder">
Game Key Art / Main Screenshot
</div>
</section>

<section>
<h2>Main Features</h2>

<div class="grid">

<div class="card">
<h3>Asymmetric Multiplayer</h3>
<p>Survivors and monsters play differently, creating tense matches.</p>
</div>

<div class="card">
<h3>Light & Vision Mechanics</h3>
<p>Dynamic lighting affects visibility, movement, and survival.</p>
</div>

<div class="card">
<h3>Cooperative Gameplay</h3>
<p>Players must communicate and coordinate to survive.</p>
</div>

<div class="card">
<h3>Multiple Game Modes</h3>
<p>Survival, Zombie, and Escape modes offer different challenges.</p>
</div>

</div>
</section>

<section>
<h2>Characters</h2>

<div class="grid">

<div class="card">
<h3>Survivors</h3>
<ul>
<li>Dynamic flashlights</li>
<li>Manual light control</li>
<li>Slower movement</li>
<li>Unique player colors</li>
</ul>
</div>

<div class="card">
<h3>Monsters</h3>
<ul>
<li>Faster movement</li>
<li>Unique playstyles</li>
<li>Larger presence</li>
<li>Eliminate survivors</li>
</ul>
</div>

</div>

<div class="image-placeholder">
Character Concepts / In-Game Models
</div>

</section>

<section>
<h2>Game Modes</h2>

<div class="grid">

<div class="card">
<h3>Survival Mode</h3>
<p>Monsters eliminate survivors before time expires.</p>
</div>

<div class="card">
<h3>Zombie Mode</h3>
<p>Eliminated survivors become monsters.</p>
</div>

<div class="card">
<h3>Escape Mode</h3>
<p>Repair objectives and escape before time runs out.</p>
</div>

</div>
</section>

<section>
<h2>Maps</h2>

<ul>
<li>Villa</li>
<li>Cemetery</li>
<li>Laboratory</li>
<li>Forest (Via dei Ronchi)</li>
</ul>

<div class="image-placeholder">
Map Screenshots / Environment Art
</div>

</section>

<section>
<h2>Game Screenshots</h2>

<p>Take a look at gameplay moments from Seescape.</p>

<div class="grid screenshots">

<img src="images/screenshot1.jpg" alt="Seescape gameplay screenshot 1">
<img src="images/screenshot2.jpg" alt="Seescape gameplay screenshot 2">
<img src="images/screenshot3.jpg" alt="Seescape gameplay screenshot 3">
<img src="images/screenshot4.jpg" alt="Seescape gameplay screenshot 4">

</div>

</section>

<section>
<h2>Customization</h2>

<div class="grid">

<div class="card">
<h3>Avatar Customization</h3>
<ul>
<li>Visual customization</li>
<li>Unlockable cosmetics</li>
<li>Player identity</li>
</ul>
</div>

<div class="card">
<h3>Cosmetics & Progression</h3>
<ul>
<li>Skins</li>
<li>Emotes</li>
<li>Limited items</li>
<li>Season Pass rewards</li>
</ul>
</div>

</div>

<div class="image-placeholder">
Avatar Customization
</div>

</section>

<section>
<h2>Download the Game</h2>

<p>Play Seescape on your platform.</p>

<div class="download-buttons">

<a href="https://drive.google.com/file/d/18A5L4clfM66sOVld4OZt6W2mCwGAD1IO/view?usp=sharing" class="download-btn windows">
Download for Windows
</a>

<a href="https://drive.google.com/file/d/1R8v0cwVKVYSMS6osC0Y9ECT8n_U4YNJ9/view?usp=sharing" class="download-btn linux">
Download for Linux
</a>

</div>

</section>

<section>
<h2>Download via QR Code</h2>

<p>Scan a QR code with your mobile device to download Seescape instantly.</p>

<div class="grid qr-section">

<div class="card">
<h3>Windows Download</h3>
<img src="images/url_qrcodecreator.com_11_10_27.png" alt="QR code for Windows download">
<p>Scan to download the Windows version.</p>
</div>

<div class="card">
<h3>Linux Download</h3>
<img src="images/download linux.png" alt="QR code for Linux download">
<p>Scan to download the Linux version.</p>
</div>

</div>

</section>

<footer>
© Seescape — Multiplayer Survival Game<br>
Designed for Mobile & PC
</footer>

<!-- ===================== -->
<!-- COOKIE CONSENT BANNER -->
<!-- ===================== -->

<div id="cookie-banner">
This website uses cookies to improve user experience.
<button onclick="acceptCookies()">Accept</button>
</div>

<script>

/* Set Cookie */
function setCookie(name, value, days) {
    let expires = "";
    if (days) {
        const date = new Date();
        date.setTime(
            date.getTime() + (days*24*60*60*1000)
        );
        expires = "; expires=" + date.toUTCString();
    }
    document.cookie =
        name + "=" + value + expires + "; path=/";
}

/* Get Cookie */
function getCookie(name) {
    const cookies = document.cookie.split("; ");
    for (let cookie of cookies) {
        const parts = cookie.split("=");
        if (parts[0] === name) {
            return parts[1];
        }
    }
    return null;
}

/* Accept Cookies */
function acceptCookies() {
    setCookie("cookieConsent", "true", 365);
    document.getElementById(
        "cookie-banner"
    ).style.display = "none";
}

/* Check Consent */
window.onload = function () {
    if (getCookie("cookieConsent") === "true") {
        document.getElementById(
            "cookie-banner"
        ).style.display = "none";
    }
};

</script>

</body>
</html>
