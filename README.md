<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Samba | Web Developer</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background: #0f172a;
  color: white;
  scroll-behavior: smooth;
}

/* NAVBAR */
nav {
  position: sticky;
  top: 0;
  background: #020617;
  display: flex;
  justify-content: center;
  gap: 30px;
  padding: 15px;
  z-index: 1000;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
  transition: 0.3s;
}

nav a:hover {
  color: #38bdf8;
}

/* HERO */
header {
  text-align: center;
  padding: 80px 20px;
}

header h1 {
  font-size: 42px;
}

header p {
  margin-top: 10px;
  color: #94a3b8;
}

/* SECTIONS */
section {
  padding: 60px 20px;
  max-width: 900px;
  margin: auto;
}

h2 {
  margin-bottom: 20px;
}

/* CARDS */
.card {
  background: #1e293b;
  padding: 20px;
  margin: 15px 0;
  border-radius: 12px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-5px);
  background: #334155;
}

/* BUTTON */
.btn {
  display: inline-block;
  margin-top: 10px;
  padding: 10px 15px;
  background: #38bdf8;
  color: black;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
}

/* FOOTER */
footer {
  text-align: center;
  padding: 20px;
  background: #020617;
  margin-top: 40px;
}

/* FADE ANIMATION */
.fade {
  opacity: 0;
  transform: translateY(20px);
  transition: 1s;
}

.fade.show {
  opacity: 1;
  transform: translateY(0);
}
</style>
</head>

<body>

<nav>
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#projects">Projects</a>
  <a href="#contact">Contact</a>
</nav>

<header id="home" class="fade">
  <h1>Hi, I'm Samba 👋</h1>
  <p>Web Developer | Building Modern Websites</p>
</header>

<section id="about" class="fade">
  <h2>About Me</h2>
  <div class="card">
    <p>
      I'm a passionate web developer focused on creating clean, responsive and user-friendly websites.
      Currently improving my skills in HTML, CSS and JavaScript.
    </p>
  </div>
</section>

<section id="projects" class="fade">
  <h2>Projects</h2>

  <div class="card">
    <h3>Portfolio Website</h3>
    <p>This is my personal portfolio hosted online.</p>
    <a href="#" class="btn">View Project</a>
  </div>

  <div class="card">
    <h3>Coming Soon</h3>
    <p>More projects will be added here.</p>
  </div>

</section>

<section id="contact" class="fade">
  <h2>Contact</h2>
  <div class="card">
    <p>Email: bachjawo11@gmail.come</p>
    <p>Phone: +220 7597080</p>
  </div>
</section>

<footer>
  <p>© 2026 Samba. All rights reserved.</p>
</footer>

<script>
const faders = document.querySelectorAll('.fade');

window.addEventListener('scroll', () => {
  faders.forEach(el => {
    const top = el.getBoundingClientRect().top;
    if (top < window.innerHeight - 100) {
      el.classList.add('show');
    }
  });
});
</script>

</body>
</html>
