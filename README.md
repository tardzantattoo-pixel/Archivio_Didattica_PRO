# Archivio_Didattica_PRO
<!DOCTYPE html>
<html lang="it">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Archivio Didattica Biennio</title>

<link rel="manifest" href="manifest.json">
<meta name="theme-color" content="#1e293b">

<link rel="stylesheet" href="style.css">
</head>

<body>

<div class="layout">

  <aside class="sidebar">
    <h2>Archivio</h2>
    <button onclick="goHome()">🏠 Dashboard</button>
    <button onclick="openYear('Primo')">🎨 Primo Anno</button>
    <button onclick="openYear('Secondo')">🖌 Secondo Anno</button>
    <hr>
    <button onclick="toggleTheme()">🌙 Tema</button>
    <button onclick="backup()">💾 Backup</button>
  </aside>

  <main class="content">
    <div id="breadcrumb"></div>
    <div id="app"></div>
  </main>

</div>

<script src="app.js"></script>

<script>
if ("serviceWorker" in navigator) {
  navigator.serviceWorker.register("service-worker.js");
}
</script>

</body>
</html>
