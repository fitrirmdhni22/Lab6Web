Lab6Web
Praktikum 6

|                |                    |
| -------------- | ------------------ |
|      _Nama_    | Fitri Ramadhani |
|      _NIM_     |      312410085     |
|     _Kelas_    |      TI.24.A.1      |
|  _Mata Kuliah_ | Pemrograman Web 1 |

# INPUT PROGRAM
```HTML
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Layout Sederhana</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div id="container">
    <header>
      <h1>Layout Sederhana</h1>
    </header>

    <nav>
      <a href="home.html" class="active">Home</a>
      <a href="artikel.html">Artikel</a>
      <a href="about.html">About</a>
      <a href="kontak.html">Kontak</a>
    </nav>

    <section id="hero">
      <h1>Hello World!</h1>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu.
      </p>
      <a href="#" class="btn btn-large">Learn more »</a>
    </section>

    <section id="wrapper">
      <section id="main">
        <div class="row">
          <div class="box">
            <img src="https://dummyimage.com/120/db7d25/fff.png" class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
          </div>
          <div class="box">
            <img src="https://dummyimage.com/120/3e73e6/fff.png" class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
          </div>
          <div class="box">
            <img src="https://dummyimage.com/120/71e6d4/fff.png" class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
          </div>
        </div>

        <hr class="divider">

        <article class="entry">
          <h2>First featurette heading.</h2>
          <img src="https://dummyimage.com/150/7b8a70/fff.png">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu.
          </p>
        </article>

        <hr class="divider">

        <article class="entry">
          <h2>Second featurette heading.</h2>
          <img src="https://dummyimage.com/150/7b8a70/fff.png" class="right-img">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu.
          </p>
        </article>
      </section>

      <aside id="sidebar">
        <div class="widget-box">
          <h3 class="title">Widget Header</h3>
          <ul>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
          </ul>
        </div>

        <div class="widget-box">
          <h3 class="title">Widget Text</h3>
          <p>
            Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta.
          </p>
        </div>
      </aside>
    </section>

    <footer>
      <p>&copy; 2025 - Universitas Pelita Bangsa</p>
    </footer>
  </div>
</body>
</html>
```

# OUTPUT PROGRAM
<img width="1366" height="720" alt="image" src="https://github.com/user-attachments/assets/5411b2e5-5056-4a67-b678-14d74cde699a" />

# layout web sederhana menggunakan css frameword (Twitter Bootsrtap).
# INPUT PROGRAM
```HTML
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Home | Fitri Ramadhani - Teknik Informatika</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      scroll-behavior: smooth;
      background-color: #f8f9fa;
    }

    /* Navbar */
    nav.navbar {
      background: linear-gradient(90deg, #0d6efd, #6610f2);
    }
    nav a.nav-link {
      color: #fff !important;
      font-weight: 500;
      margin: 0 8px;
      transition: 0.3s;
    }
    nav a.nav-link:hover {
      color: #ffe082 !important;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(120deg, #0d6efd, #6f42c1);
      color: white;
      padding: 120px 20px;
      text-align: center;
      border-radius: 0 0 40px 40px;
    }
    .hero h1 {
      font-size: 3rem;
      font-weight: 700;
    }
    .hero p {
      font-size: 1.2rem;
      margin-top: 10px;
      color: #f8f9fa;
    }

    /* Feature Cards */
    .feature-card {
      background: white;
      border: none;
      border-radius: 15px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.08);
      padding: 25px;
      transition: 0.3s;
    }
    .feature-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
    }
    .feature-icon {
      width: 80px;
      height: 80px;
      background-color: #e9ecef;
      color: #0d6efd;
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 36px;
      margin: 0 auto 15px;
    }

    /* Footer */
    footer {
      background-color: #0d6efd;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 80px;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark fixed-top shadow">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">Fitri<span style="color:#ffe082;">Ramadhani</span></a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link active" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="artikel.html">Artikel</a></li>
          <li class="nav-item"><a class="nav-link" href="about.html">About</a></li>
          <li class="nav-item"><a class="nav-link" href="kontak.html">Kontak</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero mt-5">
    <div class="container">
      <h1>Selamat Datang di Dunia Teknologi 💻</h1>
      <p>Hai, aku <strong>Fitri Ramadhani</strong> — Mahasiswi Teknik Informatika yang mencintai dunia pemrograman, desain, dan inovasi digital.</p>
      <a href="about.html" class="btn btn-light btn-lg mt-3">Kenali Aku Lebih Jauh »</a>
    </div>
  </section>

  <!-- Main Content -->
  <div class="container my-5">
    <div class="text-center mb-5">
      <h2 class="fw-bold text-primary">Bidang Keahlian</h2>
      <p class="text-muted">Berikut beberapa bidang yang aku kuasai dalam dunia Teknik Informatika.</p>
    </div>

    <div class="row g-4">
      <div class="col-md-4">
        <div class="feature-card text-center">
          <div class="feature-icon"><i class="bi bi-code-slash"></i></div>
          <h5 class="fw-bold">Web Development</h5>
          <p>Membuat website interaktif dan responsif menggunakan HTML, CSS, Bootstrap, dan JavaScript.</p>
        </div>
      </div>

      <div class="col-md-4">
        <div class="feature-card text-center">
          <div class="feature-icon"><i class="bi bi-braces"></i></div>
          <h5 class="fw-bold">Pemrograman</h5>
          <p>Berpengalaman dalam pemrograman Python, PHP, dan Java dengan pendekatan logika dan efisiensi.</p>
        </div>
      </div>

      <div class="col-md-4">
        <div class="feature-card text-center">
          <div class="feature-icon"><i class="bi bi-cpu"></i></div>
          <h5 class="fw-bold">Artificial Intelligence</h5>
          <p>Belajar mengimplementasikan AI sederhana untuk analisis data dan chatbot menggunakan Python.</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Call To Action -->
  <section class="py-5 text-center bg-light">
    <div class="container">
      <h2 class="fw-bold text-primary">Mari Berkarya Bersama 🚀</h2>
      <p class="text-muted">Aku percaya teknologi bisa mengubah dunia. Yuk, mulai berinovasi hari ini!</p>
      <a href="kontak.html" class="btn btn-primary btn-lg mt-2">Hubungi Aku Sekarang</a>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Fitri Ramadhani | Teknik Informatika - Universitas Pelita Bangsa</p>
  </footer>

  <!-- Bootstrap & Icons -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.css">
</body>
</html>
```

# OUTPUT PROGRAM
<img width="1366" height="720" alt="PEMWEB2" src="https://github.com/user-attachments/assets/14bb0173-8de1-4ab4-9d4e-d7df0e39143a" />

# Terima Kasih
