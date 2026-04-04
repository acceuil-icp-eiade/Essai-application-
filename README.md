<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Livret IADE</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>

<div class="sidebar">
  <h2>🩺 IADE</h2>
  <a href="#">Accueil</a>
  <a href="#">Chirurgie</a>
  <a href="#">Urgences</a>
</div>

<div class="main">

  <header>
    <input type="text" id="search" placeholder="🔍 Rechercher...">
    <button onclick="toggleDark()">🌙</button>
  </header>

  <div class="container">

    <a href="pages/chir-cardiaque.html" class="card">
      ❤️ Chirurgie cardiaque
    </a>

    <a href="pages/urgences.html" class="card">
      🚨 Urgences
    </a>

  </div>

</div>

<script src="script.js"></script>


</html>
body {
  margin: 0;
  font-family: sans-serif;
  display: flex;
  background: #f4f7fb;
}

/* SIDEBAR */
.sidebar {
  width: 220px;
  background: #2c3e50;
  color: white;
  height: 100vh;
  padding: 20px;
}

.sidebar a {
  display: block;
  color: white;
  text-decoration: none;
  margin: 15px 0;
}

/* MAIN */
.main {
  flex: 1;
}

/* HEADER */
header {
  display: flex;
  justify-content: space-between;
  padding: 15px;
  background: white;
}

/* CARDS */
.container {
  padding: 20px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

.card {
  background: white;
  padding: 25px;
  border-radius: 15px;
  text-decoration: none;
  color: black;
}

/* DARK MODE */
.dark {
  background: #1e272e;
  color: white;
}

.dark .card {
  background: #2f3640;
  color: white;
}
// MODE SOMBRE
function toggleDark() {
  document.body.classList.toggle("dark");
}
</body>
