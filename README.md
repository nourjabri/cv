  <!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Nour Jabri - Portfolio</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <nav>
      <div class="nav-title">Nour Jabri</div>
      <ul>
      <li>
        <a href="#projects">Projects</a>
      </li>
      <li>
        <a href="#skills">Skills</a>
      </li>
      <li>
        <a href="#contact">Contact</a>
      </li>
      </ul>
    </nav>
    <!-- Hero Section -->
    <section class="hero">
      <div class="hero-content">
        <h1 class="animate-fade">Hi, I'm <span>Nour Jabri</span></h1>
        <p class="animate-slide">Flutter Developer | Junior Web Developer  </p>
        <a href="#projects" class="btn animate-pop">View My Projects</a>
      </div>
    </section>

    <!-- Projects Section --> 
    <section id="projects" class="projects">
      <h2 class="section-title">My Projects</h2>
      <div class="project-grid">
        <div class="project-card animate-card">

          <h3>Restaurant Management App</h3>
          <p>A complete restaurant ordering system built with Flutter and intergrate with Firebase.</p>
          <img scr="assets/projects/Restaurant/1.jpg" alt="Welcome Screen" data-project="restaurant">
        </div>

        <div class="project-card animate-card">
          <h3>School Management App</h3>
          <p>Mobile application for managing school operations and communication.</p>
        </div>

        <div class="project-card animate-card">
          <h3>Hadith Memorization App</h3>
          <p>A Flutter app designed to help users memorize Hadiths interactively.</p>
        </div>
      </div>
    </section>
  <section id="skills" class="skills">
    <h2 class="skills-title">Skills</h2>
    <div class="skills-card">
  <p> Flutter & Dart</p>
    <p>State Management</p>
    <p>Firebase & Subabase</p>
    <p>Rest APIs</p>
    </div>
  
    
  </section>
    <!-- Contact Section -->
    <section id ="contact"class="contact">
      <h2 class="section-title">Contact Me</h2>
      <p>Email: nourjabri19@gmail.com</p>
    <p>Phone: +963986978937</p>
      <a href="https://www.linkedin.com/in/nour-jabri-b72042115/" target="_blank">linkedin</a>
  <a href="https://github.com/nourjabri/flutter-projects" target="_blank"> GitHub</a>
    
    </section>

    <script src="script.js"></script>
  </body>
  </html>

  /* Basic Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Segoe UI", sans-serif;
}

body {
  background: #f8f9fb;
  color: #222;
  line-height: 1.6;
  overflow-x: hidden;
}
nav ul li a:hover {
  color: #6a11cb;
}
 nav ul li a {
        text-decoration: none;
  color: #333;
  font-size: 1.1rem;
  font-weight: 600;
  transition: color 0.3s ease;
}
nav ul {
    display: flex;
    list-style: none;
    gap: 20px;
    padding: 0;
    margin: 0;
}
nav{
        display: flex;
        justify-content: space-between;
    unicode-bidi: isolate;
    align-items: center;
    padding: 20px 40px;
}
.nav-title{ 
  font-size: 1.8rem;
  font-weight: 700;
  background: linear-gradient(to bottom right, #6a11cb, #2575fc);
  -webkit-background-clip: text;
  color: transparent;
}
/* Hero Section */
.hero {
  height: 80vh;
  background: linear-gradient(to bottom right, #6a11cb, #2575fc);
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 0 20px;
}

.hero h1 {
  font-size: 3rem;
  color: #fff;
  margin-bottom: 10px;
}

.hero h1 span {
  color: #ffe082;
}

.hero p {
  color: #e3e3e3;
  font-size: 1.2rem;
  margin-bottom: 20px;
}

.btn {
  background: #ffe082;
  padding: 12px 25px;
  border-radius: 25px;
  text-decoration: none;
  font-weight: bold;
  color: #333;
  transition: 0.3s;
}

.btn:hover {
  background: #fff;
  transform: scale(1.05);
}

/* Projects Section */
.projects {
  padding: 80px 20px;
  text-align: center;
}

.section-title {
  font-size: 2rem;
  margin-bottom: 40px;
  color: #e9b61d;
}
.skills-title{
    color: #e9b61d;
    font-size: 2rem;
    text-align: center;
}

.skills-card{
    display: grid;
    gap: 15px;
     color: #2575fc;
     font-weight: bold;
    max-width: 500;
    font-size: 1.5rem;
    text-align: center;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      padding: 20;
}
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 25px;
  max-width: 1100px;
  margin: auto;
}

.project-card {
  background: #fff;
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
  transition: 0.3s;
}

.project-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 25px rgba(0, 0, 0, 0.15);
}

.project-card h3 {
  color: #2575fc;
  margin-bottom: 10px;
}

/* Contact Section */
.contact {
  padding: 60px 20px;
  text-align: center;
  background: #fafafa;
}

.contact p {
  margin: 10px 0;
  font-size: 1rem;
}

/* Animations */
.animate-fade {
  animation: fadeIn 1.6s ease forwards;
  opacity: 0;
}

.animate-slide {
  animation: slideUp 1.6s ease forwards;
  opacity: 0;
}

.animate-pop {
  animation: popIn 1.8s ease forwards;
  opacity: 0;
}

.animate-card {
  animation: fadeUp 1.2s ease forwards;
  opacity: 0;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes slideUp {
  from { transform: translateY(20px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

@keyframes popIn {
  0% { transform: scale(0.8); opacity: 0; }
  100% { transform: scale(1); opacity: 1; }
}

@keyframes fadeUp {
  from { transform: translateY(30px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

