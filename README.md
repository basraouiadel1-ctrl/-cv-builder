# -cv-builder
Create and download professional CVs online”
<!DOCTYPE html>
<html>
<head>
  <title>CV Builder</title>
  <style>
    body { font-family: Arial; padding: 20px; }
    input, textarea { display: block; margin: 10px 0; width: 100%; }
    button { padding: 10px 20px; }
  </style>
</head>
<body>
  <h1>CV Builder</h1>
  <input type="text" id="name" placeholder="Your Name">
  <textarea id="experience" placeholder="Your Experience"></textarea>
  <button onclick="generateCV()">Generate CV</button>
  <pre id="output"></pre>

  <script>
    function generateCV() {
      const name = document.getElementById('name').value;
      const exp = document.getElementById('experience').value;
      document.getElementById('output').textContent = `Name: ${name}\nExperience:\n${exp}`;
    }
  </script>
</body>
</html>
