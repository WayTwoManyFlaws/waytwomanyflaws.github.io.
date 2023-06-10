<!DOCTYPE html>
<html>
<head>
  <title>SkySMP</title>
    <link rel="icon" href="website-logo.png" type="image/png">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background-color: #bae8ff;
    }
       link[rel="icon"] {
      width: 32px;
      height: 32px;
    }
    .navbar {
      background-color: #54aaff;
      text-align: center;
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 0px; /* Adjust the margin as needed */
      padding: 10px 0; /* Adjust the padding as needed */
    }
    
    .navbar .title-image {
      height: 200px;
      width: 200px;
      background-image: url("title-picture.png");
      background-repeat: no-repeat;
      background-position: center;
      background-size: contain;
      flex: 1; /* Take up remaining space */
    }
    
    .server-container {
      display: flex;
      align-items: center;
    }
    
    .server-button {
      background-color: #1d6dcf;
      border: none;
      color: #fff;
      padding: 10px 20px;
      text-decoration: none;
      font-weight: bold;
      display: flex;
      align-items: center;
      position: relative; /* Add relative positioning */
    }
    
    .server-button:hover .tooltip {
      visibility: visible; /* Show the tooltip on hover */
    }
    
    .server-button:focus {
      outline: none;
    }
    
    .copy-icon {
      height: 16px;
      width: 16px;
      margin-right: 5px;
      background-size: auto; /* Prevent stretching */
    }
    
    /* Tooltip styling */
    .tooltip {
      visibility: hidden;
      background-color: rgba(0, 0, 0, 0.8);
      color: #fff;
      text-align: center;
      border-radius: 4px;
      padding: 5px;
      position: absolute;
      bottom: 125%;
      left: 50%;
      transform: translateX(-50%);
      white-space: nowrap;
      font-size: 12px;
    }
    
    .tooltip:before {
      content: "";
      position: absolute;
      top: 100%;
      left: 50%;
      margin-left: -5px;
      border-width: 5px;
      border-style: solid;
      border-color: transparent transparent rgba(0, 0, 0, 0.8) transparent;
    }
    
    .bar {
      background-color: #1d6dcf;
      padding: 10px;
      color: #fff;
      display: flex;
      align-items: center;
    }
    
    .join-button {
      display: inline-block;
      padding: 10px;
      background-color: transparent;
      border: none;
      text-decoration: none;
      color: #fff;
      transition: color 0.3s;
      font-size: 20px;
      font-weight: bold;
    }
    
    .join-button img {
      vertical-align: middle;
      margin-right: 5px;
      height: 25px;
      width: 31px;
    }
    
    .join-button:hover {
      color: #a8c9ff;
    }
    
    .join-button:focus {
      outline: none;
    }
    
    .bottom-bar {
      background-color: #1d6dcf;
      padding: 10px;
      text-align: center;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
    
    .bottom-bar p {
      margin: 0;
      color: #fff;
      font-size: 14px;
      padding-left: 20px;
    }
    
    /* Text styling */
    h1, p, h2, ul, li {
      color: #333;
      font-size: 16px;
      line-height: 1.5;
    }
    
    h1 {
      font-size: 24px;
      font-weight: bold;
      padding-left: 10px;
    }
    
    p {
      padding-left: 20px;
    }
    
    h2 {
      font-size: 20px;
      font-weight: bold;
      padding-left: 10px;
    }
    
    ul {
      padding-left: 40px;
      list-style-type: none;
    }
    
    li {
      position: relative;
      padding-left: 20px;
    }
    
    li:before {
      content: "";
      position: absolute;
      left: 0;
      top: 8px;
      width: 6px;
      height: 6px;
      background-color: #1d6dcf;
      border-radius: 50%;
    }

    
  </style>
  <script>
    function copyToClipboard() {
      var textField = document.createElement('textarea');
      textField.innerText = 'skysmp.de';
      document.body.appendChild(textField);
      textField.select();
      document.execCommand('copy');
      textField.remove();
      alert('Copied server IP to clipboard: skysmp.de');
    }
  </script>
</head>
<body>
  <div class="navbar">
    <div class="server-container">
      <button class="server-button" onclick="copyToClipboard()">
        <img class="copy-icon" src="copy-icon.png" alt="Copy Icon">
        ServerIP: SkySMP.de
        <span class="tooltip">Copy to clipboard!</span>
      </button>
    </div>
    <div class="title-image"></div>
  </div>
  
  <div class="bar">
    <a href="https://discord.gg/mzEEFNRG5" class="join-button">
      <img src="discord-icon.png" alt="Discord Icon">
      <strong>Join our Discord!</strong>
    </a>
  </div>
  
  <h1>Wilkommen zum offiziellen SkySMP!</h1>
  <p>Diese Website gehört zum SkySMP.de Minecraft Server</p>
  <p>Dieser läuft auf der 1.20 Version und ist als gemütlicher Survival Multiplayer gedacht.
   Falls du mehr über den Server erfahren willst, joine doch gerne unserem Discord Server.</p>
  <h2>Wie kann man dem Server joinen?</h2>
  <p>Da der Server zu diesem Zeitpunkt noch neu ist, kannst du einfach auf den Discord kommen und dich von dort bewerben!</p>
  <h2>Anforderungen:</h2>
  <ul>
    <li>Minecraft Java haben</li>
    <li>Discord auf dem PC installiert haben</li>
    <li>Mikrofon/Headset besitzen</li>
    <li>Regeln akzeptieren und mindestens 13 Jahre alt sein</li>
  </ul>
  <h2>Regeln:</h2>
  <ul>
    <li>Sei respektvoll und beleidige niemanden</li>
    <li>Halte dich an die Regeln im Discord Server</li>
    <li>Nutze keine Exploits, Hackclients oder andere Cheats, die dir einen unfairen Vorteil verschaffen</li>
    <li id="fourth-rule">Respektiere die Farmen, Territorien und Gebäude anderer auf dem Server</li>
  </ul>
  <div class="bottom-bar">
    <p>&copy; 2023 SkySMP. All rights reserved.</p>
  </div>
</body>
</html>


