

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Professional home maintenance services in Cairo, Egypt. Plumbing, electrical, water heaters and more.">
<title>Cairo Home Maintenance | Egypt</title>

<style>
* {
  box-sizing: border-box;
}
body {
  margin: 0;
  font-family: Arial, sans-serif;
  color: #263445;
  background: #f4f8fc;
  line-height: 1.6;
}
header {
  background: #073b66;
  color: white;
  text-align: center;
  padding: 35px 15px;
}
header h1 {
  font-size: 30px;
  margin: 0;
}
nav {
  background: #0866a5;
  padding: 13px;
  text-align: center;
}
nav a {
  color: white;
  text-decoration: none;
  margin: 0 10px;
  font-weight: bold;
}
.hero {
  padding: 65px 20px;
  text-align: center;
  background: linear-gradient(135deg,#dceeff,#ffffff);
}
.hero h2 {
  font-size: 32px;
  color: #073b66;
}
.btn {
  display: inline-block;
  background: #16a34a;
  color: white;
  padding: 14px 25px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: bold;
  margin-top: 15px;
}
section {
  padding: 35px 18px;
  max-width: 1050px;
  margin: auto;
}
h2 {
  color: #073b66;
  text-align: center;
}
.services {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(210px,1fr));
  gap: 18px;
}
.service {
  background: white;
  padding: 22px;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 3px 12px #00000010;
}
.service span {
  font-size: 35px;
}
.areas {
  text-align: center;
  line-height: 2;
}
form {
  background: white;
  padding: 22px;
  border-radius: 12px;
  max-width: 550px;
  margin: auto;
}
input, select, textarea {
  width: 100%;
  padding: 13px;
  margin: 8px 0;
  border: 1px solid #ccd5df;
  border-radius: 6px;
  font-size: 15px;
}
button {
  width: 100%;
  padding: 14px;
  background: #16a34a;
  color: white;
  border: 0;
  border-radius: 7px;
  font-size: 17px;
  cursor: pointer;
}
footer {
  background: #073b66;
  color: white;
  text-align: center;
  padding: 25px;
}
</style>
</head>

<body>

<header>
  <h1>CAIRO HOME MAINTENANCE</h1>
  <p>Professional Home Services in Egypt</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#services">Services</a>
  <a href="#areas">Areas</a>
  <a href="#contact">Contact</a>
</nav>

<div class="hero" id="home">
  <h2>Your Trusted Home Maintenance Partner in Cairo</h2>
  <p>Professional Plumbing, Electrical and Home Repair Services.</p>
  <p>Reliable Service • Experienced Technicians • 1-Month Warranty</p>
  <a class="btn" href="#contact">REQUEST A SERVICE</a>
</div>

<section id="services">
  <h2>Our Services</h2>
  <div class="services">

    <div class="service">
      <span>🚿</span>
      <h3>Plumbing</h3>
      <p>Installation, repairs and water leak solutions.</p>
    </div>

    <div class="service">
      <span>⚡</span>
      <h3>Electrical</h3>
      <p>Home electrical repairs and installations.</p>
    </div>

    <div class="service">
      <span>🔥</span>
      <h3>Water Heaters</h3>
      <p>Water heater maintenance and repairs.</p>
    </div>

    <div class="service">
      <span>❄️</span>
      <h3>Air Conditioning</h3>
      <p>AC maintenance and installation.</p>
    </div>

    <div class="service">
      <span>🔨</span>
      <h3>Carpentry</h3>
      <p>Doors, furniture and home repairs.</p>
    </div>

    <div class="service">
      <span>🏠</span>
      <h3>General Maintenance</h3>
      <p>Complete home maintenance solutions.</p>
    </div>

  </div>
</section>

<section id="areas">
  <h2>Our Service Areas</h2>
  <div class="areas">
    Heliopolis • Nasr City • Zamalek<br>
    Maadi • Dokki • Mohandessin<br>
    New Cairo • Cairo and Surrounding Areas
  </div>
</section>

<section id="contact">
  <h2>Request a Service</h2>
  <p style="text-align:center">
    Fill in the form and send your request directly to WhatsApp.
  </p>

  <form onsubmit="sendWhatsApp(event)">
    <input id="name" placeholder="Full Name" required>
    <input id="phone" placeholder="Your Phone Number" required>

    <select id="service" required>
      <option value="">Select a Service</option>
      <option>Plumbing</option>
      <option>Electrical</option>
      <option>Water Heaters</option>
      <option>Air Conditioning</option>
      <option>Carpentry</option>
      <option>General Maintenance</option>
    </select>

    <input id="area" placeholder="Your Area" required>
    <input id="address" placeholder="Full Address">

    <textarea id="details" placeholder="Describe Your Problem"></textarea>

    <button type="submit">SEND REQUEST VIA WHATSAPP</button>
  </form>
</section>

<script>
function sendWhatsApp(event) {
  event.preventDefault();

  const message =
    "New Maintenance Request\n" +
    "Name: " + document.getElementById("name").value + "\n" +
    "Phone: " + document.getElementById("phone").value + "\n" +
    "Service: " + document.getElementById("service").value + "\n" +
    "Area: " + document.getElementById("area").value + "\n" +
    "Address: " + document.getElementById("address").value + "\n" +
    "Details: " + document.getElementById("details").value;

  const url = "https://wa.me/201004220919?text=" +
              encodeURIComponent(message);

  window.open(url, "_blank");
}
</script>

<footer>
  <h3>CAIRO HOME MAINTENANCE</h3>
  <p>Professional Home Services in Egypt</p>
  <p>WhatsApp: +20 100 422 0919</p>
  <p>© 2026 All Rights Reserved</p>
</footer>

</body>
</html>
