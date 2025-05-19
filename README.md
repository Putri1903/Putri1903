<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Selamat Ulang Tahun!</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <h1>🎉 Selamat Ulang Tahun, Sayang! 🎉</h1>
    <p id="message"></p>
  </div>

  <script>
    const message = "Hari ini adalah hari spesialmu, dan aku bersyukur bisa merayakannya bersamamu. Terima kasih telah menjadi kamu yang begitu luar biasa. Semoga semua keinginanmu tercapai dan kamu selalu bahagia. Aku sayang kamu ❤️";
    let i = 0;
    const speed = 50;

    function typeWriter() {
      if (i < message.length) {
        document.getElementById("message").innerHTML += message.charAt(i);
        i++;
        setTimeout(typeWriter, speed);
      }
    }

    window.onload = typeWriter;
  </script>
</body>
</html>
