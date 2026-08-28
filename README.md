# similation-phisyng
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simulation de phishing</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: Arial, sans-serif;
      background: #111827;
      color: white;
      padding: 20px;
    }

    .card {
      width: 100%;
      max-width: 420px;
      background: #1f2937;
      border-radius: 20px;
      padding: 30px 24px;
      text-align: center;
      box-shadow: 0 15px 40px rgba(0,0,0,.35);
    }

    .icon {
      font-size: 55px;
      margin-bottom: 15px;
    }

    h1 {
      margin: 0 0 15px;
      font-size: 27px;
    }

    p {
      color: #d1d5db;
      line-height: 1.5;
    }

    .warning {
      background: #3f2b13;
      border: 1px solid #f59e0b;
      color: #fbbf24;
      padding: 15px;
      border-radius: 12px;
      margin: 20px 0;
    }

    button {
      width: 100%;
      padding: 14px;
      border: 0;
      border-radius: 12px;
      background: #2563eb;
      color: white;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
    }

    #message {
      display: none;
      margin-top: 20px;
      color: #86efac;
      font-weight: bold;
    }

    small {
      display: block;
      margin-top: 20px;
      color: #9ca3af;
    }
  </style>
</head>

<body>

  <div class="card">
    <div class="icon">⚠️</div>

    <h1>Simulation de phishing</h1>

    <p>
      Tu viens de cliquer sur un lien potentiellement suspect.
    </p>

    <div class="warning">
      🔒 <strong>Aucun piratage n'a eu lieu.</strong><br>
      Cette page est uniquement une démonstration.
    </div>

    <button onclick="showMessage()">
      Comprendre le danger
    </button>

    <div id="message">
      ✅ Ne donne jamais ton mot de passe, tes codes ou tes informations personnelles
      sur une page dont tu ne connais pas la provenance.
    </div>

    <small>
      Démonstration éducative — aucune donnée n'est collectée.
    </small>
  </div>

  <script>
    function showMessage() {
      document.getElementById("message").style.display = "block";
    }
  </script>

</body>
</html>