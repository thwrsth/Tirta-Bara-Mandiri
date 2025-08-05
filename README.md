<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tirta Bara Mandiri - Briket Batok Kelapa</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #fefefe;
      color: #333;
    }
    header {
      background: #222;
      color: white;
      padding: 1em;
      text-align: center;
    }
    section {
      padding: 2em;
      max-width: 800px;
      margin: auto;
    }
    h1, h2 {
      color: #8B4513;
    }
    .highlight {
      background: #ffe5b4;
      padding: 1em;
      border-radius: 8px;
      margin-top: 1em;
    }
    .contact {
      background: #f2f2f2;
      padding: 1em;
      margin-top: 2em;
      border-radius: 8px;
    }
    .cta {
      display: block;
      width: fit-content;
      margin: 2em auto 0;
      padding: 1em 2em;
      background: #8B4513;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
    }
    footer {
      text-align: center;
      font-size: 0.9em;
      padding: 1em;
      background: #eee;
    }

    /* SLIDESHOW */
    .slideshow-container {
      position: relative;
      max-width: 100%;
      margin: 2em auto;
      border-radius: 8px;
      overflow: hidden;
    }

    .slide {
      display: none;
      width: 100%;
    }

    .slide img {
      width: 100%;
      height: auto;
      display: block;
    }

    /* Next & previous buttons */
    .prev, .next {
      cursor: pointer;
      position: absolute;
      top: 50%;
      width: auto;
      padding: 16px;
      margin-top: -22px;
      color: white;
      font-weight: bold;
      font-size: 18px;
      transition: 0.3s ease;
      user-select: none;
      background-color: rgba(0,0,0,0.5);
      border-radius: 0 3px 3px 0;
    }

    .next {
      right: 0;
      border-radius: 3px 0 0 3px;
    }

    .prev:hover, .next:hover {
      background-color: rgba(0,0,0,0.8);
    }
  </style>
</head>
<body>
  <header>
    <h1>Tirta Bara Mandiri</h1>
    <p>Briket Batok Kelapa Ramah Lingkungan</p>
  </header>

  <section>
    <h2>Tentang Produk</h2>
    <p>Kami memproduksi <strong>briket batok kelapa</strong> bentuk kubus (2x2x2 cm) yang tidak berasap saat dibakar dan sangat cocok untuk keperluan memasak maupun kebutuhan industri.</p>

    <!-- SLIDESHOW -->
    <div class="slideshow-container">
      <div class="slide">
        <img src="gambar1.jpg" alt="Briket 1">
      </div>
      <div class="slide">
        <img src="gambar2.jpg" alt="Briket 2">
      </div>
      <div class="slide">
        <img src="gambar3.jpg" alt="Briket 3">
      </div>

      <a class="prev" onclick="plusSlides(-1)">❮</a>
      <a class="next" onclick="plusSlides(1)">❯</a>
    </div>
  </section>

  <footer>
    &copy; 2025 Tirta Bara Mandiri. Semua Hak Dilindungi.
  </footer>

  <script>
    let slideIndex = 1;
    showSlides(slideIndex);

    function plusSlides(n) {
      showSlides(slideIndex += n);
    }

    function showSlides(n) {
      const slides = document.getElementsByClassName("slide");
      if (n > slides.length) slideIndex = 1;
      if (n < 1) slideIndex = slides.length;
      for (let i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
      }
      slides[slideIndex - 1].style.display = "block";
    }

    // Auto play
    setInterval(() => { plusSlides(1); }, 4000);
  </script>
</body>
</html>
