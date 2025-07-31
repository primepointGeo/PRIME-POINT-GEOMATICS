<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Prime Point Geomatics</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #ffffff;
      color: #222;
    }

    header {
      background-color: #012e57;
      color: white;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      margin: 0;
    }

    nav a {
      color: white;
      margin-left: 20px;
      text-decoration: none;
      font-weight: 500;
    }

    .hero {
      background: url('https://images.unsplash.com/photo-1516574187841-cb9cc2ca948b?fit=crop&w=1600') no-repeat center center/cover;
      height: 400px;
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }

    .hero h2 {
      font-size: 3em;
      background-color: rgba(0,0,0,0.5);
      padding: 20px;
      border-radius: 10px;
    }

    .section {
      padding: 60px 40px;
      text-align: center;
    }

    .services {
      flex-wrap: wrap;
      gap: 40px;
      flex-direction: row;
      display: flex;
      justify-content: center;
    }

    .service {
      flex: 0 0 200px;
      margin: 20px;
    }

    .about {
      max-width: 800px;
      margin: auto;
      font-size: 1.1em;
    }

    footer {
      background-color: #012e57;
      color: white;
      padding: 30px 40px;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    footer p, footer a {
      margin: 5px 0;
      color: #ddd;
      text-decoration: none;
    }

    .socials a {
      margin-left: 15px;
    }

    #toggle-sound {
      position: fixed;
      bottom: 80px;
      left: 10px;
      z-index: 1000;
      padding: 10px 15px;
      background-color: #012e57;
      color: white;
      border: none;
      border-radius: 5px;
      font-weight: bold;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <header>
    <h1>PRIME POINT GEOMATICS</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#services">Services</a>
      <a href="#about">About</a>
      <a href="#">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Surveying & Geospatial Services</h2>
  </section>

  <section class="section" id="services">
    <h2>Our Services</h2>
    <div class="services">
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/theodolite.png" alt="Surveying" height="60">
        <h3>Surveying</h3>
      </div>
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/top-view.png" alt="Mapping" height="60">
        <h3>Mapping</h3>
      </div>
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/satellite.png" alt="Remote Sensing" height="60">
        <h3>Remote Sensing</h3>
      </div>
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/drone-camera.png" alt="Drone Surveying" height="60">
        <h3>Drone Surveying</h3>
      </div>
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/globe.png" alt="GIS Analysis" height="60">
        <h3>GIS Analysis</h3>
      </div>
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/city-buildings.png" alt="Engineering Survey" height="60">
        <h3>Engineering Survey</h3>
      </div>
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/ocean.png" alt="Hydrographic Survey" height="60">
        <h3>Hydrographic Survey</h3>
      </div>
      <div class="service">
        <img src="https://img.icons8.com/ios-filled/100/000000/parcel.png" alt="Cadastral Survey" height="60">
        <h3>Cadastral Survey</h3>
      </div>
    </div>
  </section>

  <section class="section about" id="about">
    <h2>About Us</h2>
    <p>
      Prime Point Geomatics is at the forefront of innovation in the field of geomatics. We provide precise surveying solutions across various sectors, utilizing drone technology and advanced GIS methods. Our mission is to enhance geospatial accuracy and deliver high-impact data to support infrastructure and environmental projects.
    </p>
  </section>

  <section class="section" id="contact">
    <h2>Contact Us</h2>
    <p>Please fill out the form below to get in touch with us.</p>
    <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfD_PLACEHOLDER_URL/viewform?embedded=true"
            width="100%" height="700" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
  </section>

  <footer>
    <div>
      <p>Abeokuta, Ogun State Nigeria</p>
      <p>(+234) 7063644157</p>
      <p>primepointgeomatics@gmail.com</p>
    </div>
    <div class="socials">
      <a href="#">Facebook</a>
      <a href="#">LinkedIn</a>
      <a href="#">Twitter</a>
    </div>
  </footer>

  <!-- Background Music + Mute Toggle -->
  <audio id="background-audio" autoplay loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/02/audio_fef362b72a.mp3?filename=inspiring-ambient-116199.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <button id="toggle-sound">Mute Music</button>

  <script>
    document.addEventListener("DOMContentLoaded", function () {
      const audio = document.getElementById("background-audio");
      const toggleBtn = document.getElementById("toggle-sound");
      toggleBtn.addEventListener("click", function () {
        audio.muted = !audio.muted;
        toggleBtn.innerText = audio.muted ? "Unmute Music" : "Mute Music";
      });
    });
  </script>

</body>
</html>
