<!DOCTYPE html>
<html>
<head>
  <title>Imagem Interativa</title>
  <style>
    #imagem {
      width: 500px;
      height: 300px;
      background-image: url('imagem1.jpg');
      background-size: cover;
    }
  </style>
</head>
<body>
  <div id="imagem"></div>
  <script>
    const imagem = document.getElementById('imagem');
    imagem.addEventListener('click', (e) => {
      const x = e.clientX;
      const y = e.clientY;
      if (x > 100 && x < 200 && y > 100 && y < 200) {
        imagem.style.backgroundImage = 'url("imagem2.jpg")';
      }
    });
  </script>
</body>
</html>
