# emirdykn.github.io
Basit renk değiştirici web sitesi
<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Renk Değişen Blok</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f0f0f0;
    }

    #blok {
      width: 200px;
      height: 200px;
      background-color: cornflowerblue;
      border-radius: 15px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
  </style>
</head>
<body>
  <div id="blok"></div>

  <script>
    const blok = document.getElementById("blok");
    let degisti = false;

    blok.addEventListener("click", () => {
      if (degisti) {
        blok.style.backgroundColor = "cornflowerblue";
        document.body.style.backgroundColor = "#f0f0f0";
      } else {
        blok.style.backgroundColor = "tomato";
        document.body.style.backgroundColor = "lightyellow";
      }
      degisti = !degisti;
    });
  </script>
</body>
</html>
