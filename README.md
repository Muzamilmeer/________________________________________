

<html lang="en">    
<head>    
  <meta charset="UTF-8" />    
  <meta name="viewport" content="width=device-width, initial-scale=.50" />    
  <title>Muzamil Streetwear | Portfolio & Store</title>    
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700&display=swap" rel="stylesheet" />    
  <style> 
.typewriter-box {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 10px;
}

.typewriter {
  display: inline-block;
  overflow: hidden;
  border-right: 3px solid #00ffff;
  white-space: normal;
  font-size: 18px;
  width: 100%;
  max-width: 600px;
  color: #fff;
  text-align: center;
  animation: typing 30s steps(100, end), blink 0.75s step-end infinite;
  line-height: 1.5;
}

@keyframes typing {
  from {
    max-width: 0;
  }
  to {
    max-width: 600px;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}   
    * {    
      margin: 0;    
      padding: 0;    
      box-sizing: border-box;    
      scroll-behavior: smooth;    
    }    
    body {    
      font-family: 'Orbitron', sans-serif;    
      background: #111;    
      color: #fff;    
    }    
    header {    
      display: flex;    
      justify-content: space-between;    
      align-items: center;    
      padding: 15px 30px;    
      background: linear-gradient(135deg, #000000, #1f1f1f);    
      box-shadow: 0 0 10px #00ffff;    
    }    
    .logo-section {    
      display: flex;    
      align-items: center;    
    }    
    .logo-img {    
      width: 100px;    
      height: 100px;    
      border-radius: 10px;    
      margin-right: 15px;    
    }    
    .logo-text {    
      font-size: 28px;    
      color: #00ffff;    
      text-shadow: 1px 1px 5px #00ffff, -1px -1px 5px #00ffff;    
      animation: glow 2s infinite alternate;    
    }    
    @keyframes glow {    
      from { text-shadow: 0 0 5px #00ffff; }    
      to { text-shadow: 0 0 15px #00ffff, 0 0 30px #0ff; }    
    }    
    .social-icons {    
      display: flex;    
      gap: 30px;    
    }    
    .social-icons img {    
      width: 100px;    
      transition: transform 0.3s ease;    
      filter: drop-shadow(0 0 4px #00ffff);    
    }    
    .social-icons img:hover {    
      transform: scale(1.2);    
    }    
    nav {    
      display: flex;    
      justify-content: center;    
      gap: 20px;    
      background: #1f1f1f;    
      padding: 10px;    
    }    
    nav a {    
      color: #00ffff;    
      text-decoration: none;    
      font-size: 18px;    
    }    
    nav a:hover {    
      color: #fff;    
    }    
    .container {    
      max-width: 1200px;    
      margin: auto;    
      padding: 40px 20px;    
    }    
    h2 {    
      text-align: center;    
      color: #00ffff;    
      margin-bottom: 20px;    
    }    
    .product-grid {    
      display: grid;    
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));    
      gap: 20px;    
    }    
    .product {    
      background: #222;    
      padding: 20px;    
      border-radius: 10px;    
      text-align: center;    
      box-shadow: 0 0 10px rgba(0,255,255,0.2);    
    }    
    .product img {    
      max-width: 100%;    
      border-radius: 10px;    
      margin-bottom: 10px;    
    }    
    .product a {    
      display: inline-block;    
      background: #25D366;    
      color: white;    
      padding: 10px 20px;    
      border-radius: 30px;    
      text-decoration: none;    
    }    
    .about, .skills, .projects, .contact {    
      margin-bottom: 60px;    
    }    
    .skills ul, .projects ul {    
      list-style: none;    
      text-align: center;    
    }    
    .skills li, .projects li {    
      margin: 10px 0;    
    }    
    .payment-section img {    
      display: block;    
      margin: 20px auto;    
      max-width: 150px;    
      border-radius: 10px;    
      box-shadow: 0 0 10px #00ffff;    
    }    
    footer {    
      text-align: center;    
      padding: 20px;    
      color: #aaa;    
      font-size: 14px;    
      background: #1a1a1a;    
    }    

  </style>    
</head>    
<body>
<body onload="playWelcome()">

<!-- Splash Screen -->
<div id="splash" style="
  position: fixed;
  top: 0; left: 0;
  width: 100%;
  height: 100%;
  background-color: #000;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;
  flex-direction: column;
">
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1744384921/IMG_20250411_202120_wx6x6n.png"
    alt="Logo"
    style="width: 130px; height: 130px; border-radius: 20px; box-shadow: 0 0 25px #00ffff; animation: pulse 5s infinite;">
  <h1 style="color: #00ffff; font-family: 'Orbitron', sans-serif; margin-top: 20px; animation: fadeIn 7s;">
    
  </h1>
</div>

<!-- Welcome Sound -->
<audio id="welcomeAudio" autoplay>
  <source src="https://res.cloudinary.com/dxjkbpmgm/video/upload/v1751381873/ttsMP3.com_VoiceText_2025-7-1_20-22-46_hcvby2.mp3" type="audio/mpeg">
</audio>

<script>
  function playWelcome() {
    const audio = document.getElementById("welcomeAudio");
    audio.play();
    setTimeout(() => {
      document.getElementById("splash").style.display = "none";
      document.getElementById("mainContent").style.display = "block";
    }, 6000); // wait 6sec
  }
</script>

<style>
  @keyframes pulse {
    0% { transform: scale(1); box-shadow: 0 0 15px #00ffff; }
    50% { transform: scale(1.1); box-shadow: 0 0 30px #00ffff; }
    100% { transform: scale(1); box-shadow: 0 0 15px #00ffff; }
  }
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
</style>

</body>

  <header>    
    <div class="logo-section">    
      <img class="logo-img" src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1744384921/IMG_20250411_202120_wx6x6n.png" alt="Muzamil Logo">    
      <div class="logo-text">Muzamil Streetwear</div>    
    </div>    
    <div class="social-icons">    
      <a href="https://www.instagram.com/mr____unstoppable___?igsh=MW5tcm93OHg4a3pv" target="_blank">    
        <img src="https://cdn-icons-png.flaticon.com/512/174/174855.png" alt="Instagram" />    
      </a>    
      <a href="https://www.snapchat.com/add/meir-muzamil" target="_blank">    
        <img src="https://cdn-icons-png.flaticon.com/512/3670/3670055.png" alt="Snapchat" />    
      </a>    
    </div>    
  </header>    <nav>    
    <a href="#products">Products</a>    
    <a href="#about">About</a>    
    <a href="#skills">Skills</a>    
    <a href="#projects">Projects</a>    
    <a href="#payment">Pay</a>    
    <a href="#contact">Contact</a>    
  </nav>    <div class="container">    
    <section id="products">    
      <h2>Shop Now</h2>    
      <div class="product-grid">    
        <div class="product">    
          <h3>Urban T-Shirt - ₹499</h3>    
          <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1744284703/urban-t-shirt-design-614_1080x_pbjxnu.jpg" alt="T-Shirt">    
          <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Urban%20T-Shirt">Buy</a>    
        </div>    
        <div class="product">    
          <h3>Jordan Shoes - ₹1499</h3>    
          <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1744284703/image_3_qwbkmd.jpg" alt="Shoes">    
          <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Jordan%20Shoes">Buy</a>    
        </div>    
        <div class="product">    
          <h3>Baggy Jeans - ₹799</h3>    
          <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1744284703/6b9e4944-ff98-4921-9989-afb5bf2518ca1733547766499-DENIMLOOK-Men-Relaxed-Fit-Stretchable-Baggy--Jeans-275173354-2_1_w3mivu.jpg" alt="Jeans">    
          <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Baggy%20Jeans">Buy</a>    
        </div>    
        <div class="product">    
          <h3>Black Hoodie - ₹999</h3>    
          <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750842569/61VA-FfFVpL._AC_SL1000__cxsgbf.jpg" alt="Hoodie">    
          <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Black%20Hoodie">Buy</a>    
        </div>    
<div class="product">  
  <h3>Denim Jacket - ₹1199</h3>  
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750851236/F7AB3223-F87B-4568-AED0-C58C41D8CF0A_1_qzham2.png" alt="Denim Jacket">  
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Denim%20Jacket">Buy</a>  
</div>  
<div class="product">  
  
  <h3>AeroDrip Vibe Sneakers – ₹1799
  </h3>  
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750851234/18722ec089cc49156a888602e31e2149_cbjr0w.jpg" alt="Socks">  
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Sneaker%20Socks">Buy</a>  
</div>  
<div class="product">  
    
  <h3>ShadowFlex Oversized Tee – ₹699</h3>  
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750851233/61DgGIeSAkL._SY606__vvzr5q.jpg" alt="Socks">  
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Sneaker%20Socks">Buy</a>  
</div>  
<div class="product">  
  <h3>Sneaker Socks - ₹199</h3>  
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750851234/81TRdxk1wnL._SY741__vwq5ea.jpg" alt="Socks">  
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Sneaker%20Socks">Buy</a>  
</div>  
<div class="product">  
  <h3>Graphic Hoodie - ₹1099</h3>  
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750851234/51wpvyKPnsL_hjomup.jpg" alt="Graphic Hoodie">  
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Graphic%20Hoodie">Buy</a>  
</div>  
<div class="product">  
  <h3>Cool Sunglasses - ₹499</h3>  
  <img src="https://res.cloudinary.com/demo/image/upload/v1750843000/sunglasses.jpg" alt="Sunglasses">  
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Sunglasses">Buy</a>  
</div>  
        <div class="product">    
          <h3>Cargo Pants - ₹899</h3>    
          <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750842569/4_65fe7265-e980-4cd7-828a-2c5e1df74595_hranzv.jpg" alt="Cargo Pants">    
          <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Cargo%20Pants">Buy</a>    
        </div>    
        <div class="product">    
          <h3>Stylish Cap - ₹299</h3>    
          <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750842834/s-l400_td9lev.jpg" alt="Cap">    
          <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Cap">Buy</a>    
        </div> <!-- Girls Collection Start -->
<div class="product">
  <h3>Floral Summer Dress – ₹899</h3>
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750946266/Z37_2_jyrg7f.jpg" alt="Girls Dress">
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Floral%20Summer%20Dress">Buy</a>
</div>

<div class="product">
  <h3>Women’s Sneakers – ₹599</h3>
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750946293/7cea218127c1ba7317d8dbeaff891916_btrpbb.jpg" alt="Women Sneakers">
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Women%20Sneakers">Buy</a>
</div>
<div class="product">
  <h3>Women’s Watch– ₹299</h3>
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750946266/49nhr_512_fblevc.webp" alt="Women Sneakers">
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Women%20Sneakers">Buy</a>
</div>
<div class="product">
  <h3>Women’s Makeup – ₹499</h3>
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750946266/811PxEGuypL_zaynux.jpg" alt="Women makeup">
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Women%20Sneakers">Buy</a>
</div>
<div class="product">
  <h3>Women’s Sneakers – ₹899</h3>
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750946293/rybaa_512_sk5wjr.webp" alt="Women Sneakers">
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Women%20Sneakers">Buy</a>
</div>

<div class="product">
  <h3>Trendy Handbag – ₹699</h3>
  <img src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750946292/spzlb_512_h3i3mx.webp" alt="Handbag">
  <a href="https://wa.me/919103594759?text=Hi%2C%20I%20want%20to%20buy%20Trendy%20Handbag%20Price%20%699">Buy</a>
</div>
<!-- Girls Collection End -->   
   
</div>  </section>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 30px; margin-top: 60px;">  
<div class="about">  
<div id="about" class="about">
  <!-- your about content -->
</div>
<!-- About Me -->
<div id="about" class="about" style="background:#1f1f1f; border-radius:15px; padding:25px; box-shadow: 0 0 10px #00ffff;">
  <h2 style="color:#00ffff; text-align:center;">About Me</h2>
  <div class="typewriter-box">
    <p id="typewriter" style="text-align:center; font-weight:bold;"></p>
<script>
  const txt = "Hey, I'm Muzamil — a passionate software developer who turns coffee into clean code. I build sleek apps, solve real-world problems, and love bringing ideas to life through tech. Currently leveling up my skills, one project at a time.";
  let i = 0;
  function type() {
    if (i < txt.length) {
      document.getElementById("typewriter").innerHTML += txt.charAt(i);
      i++;
      setTimeout(type, 20);
    }
  }
  type();
</script>
 
</div>
</div>
</div> 
  </div>    <!-- Skills -->    
<div id="skills" style="...">
  <!-- skills content -->
</div><div style="background:#1f1f1f; border-radius:15px; padding:25px; box-shadow: 0 0 10px #00ffff;">  
    <h2 style="color:#00ffff; text-align:center;">Skills</h2>  
    <ul style="list-style:none; text-align:center; color: #fff; font-weight:bold; font-size:18px;">  
      <li>✅ C</li>  
      <li>✅ HTML</li>  
      <li>✅ CSS</li>  
      <li>✅ Python</li>  
      <li>✅ Linux</li>  
    </ul>  
  </div>    <!-- Projects -->  
<div id="projects" style="...">
  <!-- projects content -->
</div>  <div style="background:#1f1f1f; border-radius:15px; padding:25px; box-shadow: 0 0 10px #00ffff;">  
    <h2 style="color:#00ffff; text-align:center;">Projects</h2>  
    <ul style="list-style:none; text-align:center; color: #fff; font-weight:bold; font-size:18px;">  
      <li>📌 To-Do App</li>  
      <li>📌 Weather App</li>  
      <li>📌 More coming soon...</li>  
    </ul>  
  </div>    <!-- Contact -->  
<div id="contact" style="...">
  <!-- contact content -->
</div>  <div style="background:#1f1f1f; border-radius:15px; padding:25px; box-shadow: 0 0 10px #00ffff; text-align:center; color: #fff;">  
    <h2 style="color:#00ffff;">Contact</h2>  
    <p>Email: muzamilmeer598@gmail.com</p>  
    <p>Phone: 9103594759</p>  
  </div>  </div>  <!-- Scan to Pay Full Width Section -->  
  <!-- Scan to Pay Compact Section -->

  <h2 style="color: #00ffff; font-size: 20px; margin-bottom: 15px;">
    Scan to Pay (PhonePe)
  </h2>
<div style="background:#1f1f1f; border-radius:75px; padding:10px; box-shadow: 0 0 10px #00ffff;">  
    <h2 style="color:#00ffff; text-align:center;">Projects</h2>  
    <ul style="list-style:none; text-align:center; color: #fff; font-weight:bold; font-size:18px;">  

  <!-- Clickable Image for Download via New Tab -->
  <a href="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750868015/IMG_20250625_214238_o0a1t8.png" target="_blank">
    <img 
      src="https://res.cloudinary.com/dxjkbpmgm/image/upload/v1750868015/IMG_20250625_214238_o0a1t8.png" 
      alt="Scanner" 
      style="width: 300%; max-width: 300px; border-radius: 75px; box-shadow: 0 0 100px #00ffff;"
    >
  </a>

  <p style="color: #fff; margin-top: 15px; font-size: 14px;">
    Secure UPI Payment to <strong>Muzamil</strong>
  </p>

  <p style="margin-top: 1px; font-size: 23px; color: #bbb;">
    📲 Tap the image to open & long-press to save
  </p>
</div>

