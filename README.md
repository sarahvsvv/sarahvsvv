
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sarah | Personal Portfolio</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap');

:root {
  --pink: #ff8fbd;
  --pink-light: #ffe0ed;
  --pink-dark: #e65391;
  --black: #171219;
  --white: #fff9fc;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Poppins', sans-serif;
  color: var(--black);
  background: var(--white);
  overflow-x: hidden;
}

a {
  color: inherit;
  text-decoration: none;
}

button {
  font: inherit;
}

nav {
  position: fixed;
  z-index: 100;
  top: 0;
  left: 0;
  width: 100%;
  padding: 18px 7%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: rgba(255,249,252,.86);
  backdrop-filter: blur(14px);
  border-bottom: 1px solid #f5dce7;
}

.logo {
  font-size: 22px;
  font-weight: 800;
  color: var(--pink-dark);
}

.nav-links {
  display: flex;
  gap: 28px;
  font-size: 13px;
  font-weight: 500;
}

.nav-links a:hover {
  color: var(--pink-dark);
}

section {
  padding: 110px 9%;
}

.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 50px;
  padding-top: 130px;
  background:
    radial-gradient(circle at 85% 35%, #ffd7e8 0, transparent 30%),
    var(--white);
}

.hero-text {
  max-width: 650px;
}

.eyebrow {
  color: var(--pink-dark);
  font-size: 13px;
  font-weight: 700;
  letter-spacing: 3px;
  text-transform: uppercase;
  margin-bottom: 18px;
}

.hero h1 {
  font-size: clamp(42px, 6vw, 76px);
  line-height: 1.12;
  letter-spacing: -3px;
}

.hero h1 span {
  color: var(--pink-dark);
}

.hero p {
  margin-top: 24px;
  max-width: 500px;
  line-height: 1.9;
  color: #746773;
  font-size: 15px;
}

.hero-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin-top: 30px;
}

.btn {
  display: inline-block;
  border-radius: 40px;
  padding: 13px 23px;
  font-size: 13px;
  font-weight: 600;
  transition: .25s;
  cursor: pointer;
}

.btn-primary {
  color: white;
  background: var(--pink-dark);
  border: 1px solid var(--pink-dark);
}

.btn-outline {
  border: 1px solid #e8b7ce;
  background: white;
}

.btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 22px #e6539125;
}

.hero-decoration {
  width: 310px;
  height: 390px;
  flex-shrink: 0;
  border-radius: 48% 48% 25px 25px;
  background: linear-gradient(145deg, #ffc6df, #ff8fbd);
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  transform: rotate(3deg);
  box-shadow: 0 25px 60px #e6539125;
}

.hero-decoration::before {
  content: "✦";
  position: absolute;
  top: 24px;
  right: 28px;
  font-size: 35px;
  color: white;
}

.hero-decoration::after {
  content: "CREATIVE • CURIOUS • LEARNING";
  position: absolute;
  bottom: 28px;
  color: white;
  font-size: 10px;
  letter-spacing: 2px;
  font-weight: 600;
}

.hero-monogram {
  font-size: 100px;
  font-weight: 800;
  color: white;
  letter-spacing: -8px;
}

/* GENERAL SECTION */

.section-heading {
  margin-bottom: 45px;
}

.section-heading .eyebrow {
  margin-bottom: 10px;
}

.section-heading h2 {
  font-size: clamp(30px, 4vw, 46px);
  letter-spacing: -1.5px;
}

.section-heading p {
  color: #827581;
  margin-top: 12px;
  line-height: 1.8;
  font-size: 14px;
}

.about {
  background: white;
}

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  align-items: center;
}

.about-card {
  background: #fff1f7;
  border: 1px solid #f9d6e5;
  border-radius: 25px;
  padding: 35px;
}

.about-card .big-number {
  font-size: 60px;
  color: var(--pink-dark);
  font-weight: 800;
  line-height: 1.2;
}

.about-card h3 {
  margin: 15px 0 10px;
}

.about-card p,
.about-copy {
  font-size: 14px;
  color: #746773;
  line-height: 1.9;
}

.about-copy p + p {
  margin-top: 15px;
}

.skills {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 22px;
}

.skill {
  background: #ffe4f0;
  color: #a93d70;
  border-radius: 30px;
  padding: 8px 13px;
  font-size: 12px;
  font-weight: 600;
}

/* PROJECTS */

.projects {
  background: #fff5fa;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 22px;
}

.project-card {
  background: white;
  border-radius: 20px;
  overflow: hidden;
  border: 1px solid #f3dce7;
  transition: .3s;
}

.project-card:hover {
  transform: translateY(-7px);
  box-shadow: 0 15px 35px #d98bae20;
}

.project-cover {
  height: 190px;
  background: linear-gradient(135deg, #ffd8e9, #ff9ec7);
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 48px;
}

.project-card:nth-child(2) .project-cover {
  background: linear-gradient(135deg, #f8d9ff, #e8b6ff);
}

.project-card:nth-child(3) .project-cover {
  background: linear-gradient(135deg, #ffe8c8, #ffb6c9);
}

.project-info {
  padding: 23px;
}

.project-info h3 {
  font-size: 17px;
  margin-bottom: 10px;
}

.project-info p {
  font-size: 12px;
  color: #827581;
  line-height: 1.8;
}

.project-type {
  display: inline-block;
  margin-top: 17px;
  font-size: 10px;
  font-weight: 700;
  letter-spacing: 1px;
  color: var(--pink-dark);
  text-transform: uppercase;
}

/* SPIDER-MAN SCROLL SECTION */

.spider-section {
  min-height: 100vh;
  padding: 0;
  position: relative;
  overflow: hidden;
  background: #171219;
  color: white;
}

.spider-sticky {
  min-height: 100vh;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 70px 9%;
}

.spider-content {
  position: relative;
  z-index: 2;
  max-width: 760px;
  text-align: center;
}

.spider-content .eyebrow {
  color: #ff8fbd;
}

.spider-content h2 {
  font-size: clamp(38px, 7vw, 80px);
  line-height: 1.08;
  letter-spacing: -3px;
}

.spider-content p {
  color: #c9bbc6;
  font-size: 14px;
  line-height: 1.9;
  max-width: 570px;
  margin: 22px auto 0;
}

.spider-visual {
  position: absolute;
  inset: 0;
  overflow: hidden;
  pointer-events: none;
}

.spider-orb {
  position: absolute;
  width: min(70vw, 650px);
  aspect-ratio: 1;
  border-radius: 50%;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%) scale(.35);
  opacity: .25;
  background:
    radial-gradient(circle, #ff8fbd 0%, #b72b69 25%, #49162f 55%, transparent 72%);
  transition: transform .1s linear;
}

.web-lines {
  position: absolute;
  inset: -30%;
  opacity: .16;
  background-image:
    repeating-radial-gradient(
      circle at 50% 50%,
      transparent 0 42px,
      #ffb7d6 43px 44px,
      transparent 45px 80px
    );
  transform: scale(1.1);
  transition: transform .1s linear;
}

.spider-symbol {
  position: absolute;
  font-size: clamp(80px, 17vw, 190px);
  color: #ff8fbd;
  opacity: .10;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%) scale(.6);
  transition: transform .1s linear;
}

/* EXPERIENCE */

.experience {
  background: white;
}

.timeline {
  max-width: 800px;
  border-left: 2px solid #f5c5db;
  margin-left: 8px;
  padding-left: 30px;
}

.timeline-item {
  position: relative;
  padding: 0 0 38px;
}

.timeline-item:last-child {
  padding-bottom: 0;
}

.timeline-item::before {
  content: "";
  position: absolute;
  left: -38px;
  top: 5px;
  width: 13px;
  height: 13px;
  background: var(--pink-dark);
  border: 4px solid #ffe4f0;
  border-radius: 50%;
}

.timeline-item .date {
  font-size: 11px;
  color: var(--pink-dark);
  font-weight: 700;
  letter-spacing: 1px;
}

.timeline-item h3 {
  margin: 9px 0;
  font-size: 19px;
}

.timeline-item p {
  color: #827581;
  font-size: 13px;
  line-height: 1.9;
}

/* CONTACT */

.contact {
  background: #fff0f7;
  text-align: center;
}

.contact .section-heading {
  margin-bottom: 25px;
}

.contact .section-heading p {
  max-width: 550px;
  margin-left: auto;
  margin-right: auto;
}

.contact-links {
  display: flex;
  justify-content: center;
  gap: 12px;
  flex-wrap: wrap;
  margin-top: 30px;
}

footer {
  padding: 25px;
  text-align: center;
  background: #171219;
  color: #d8c9d3;
  font-size: 11px;
}

/* DRAGGABLE ID CARD */

.lanyard-stage {
  position: fixed;
  z-index: 200;
  top: 65px;
  right: 35px;
  width: 220px;
  height: 350px;
  touch-action: none;
  user-select: none;
  cursor: grab;
  perspective: 1000px;
}

.lanyard-stage:active {
  cursor: grabbing;
}

.lanyard-assembly {
  position: absolute;
  top: 0;
  left: 0;
  width: 220px;
  height: 330px;
  transform:
    translate3d(var(--lanyard-x, 0px), var(--lanyard-y, 0px), 0)
    rotate(var(--lanyard-tilt, 0deg));
  transform-origin: 50% 0;
  will-change: transform;
}

.lanyard-ribbon {
  position: absolute;
  top: -65px;
  left: 50%;
  width: 100%;
  height: 180px;
  transform: translateX(-50%);
  filter: drop-shadow(1px 4px 3px #00000030);
}

.lanyard-ribbon::before,
.lanyard-ribbon::after {
  content: "";
  position: absolute;
  top: 0;
  height: 180px;
  width: 25px;
  border-radius: 4px 4px 2px 2px;
  background:
    repeating-linear-gradient(
      0deg,
      transparent 0px,
      #ffffff17 2px,
      transparent 4px,
      #0000000c 6px
    ),
    linear-gradient(
      90deg,
      #b8316c 0%,
      #f57eaf 13%,
      #ffafd0 32%,
      #f879ad 53%,
      #c63d78 78%,
      #86234e 100%
    );
  border-left: 1px solid #ffffff30;
  border-right: 2px solid #84204a70;
  box-shadow:
    inset 2px 0 2px #ffffff40,
    inset -3px 0 4px #6d12384a;
  transform-origin: 50% 0;
}

.lanyard-ribbon::before {
  left: 73px;
  transform: rotate(-19deg);
}

.lanyard-ribbon::after {
  left: 122px;
  transform: rotate(19deg);
}

.lanyard-hook {
  position: absolute;
  top: 93px;
  left: 50%;
  width: 34px;
  height: 30px;
  transform: translateX(-50%);
  border: 5px solid #d6d6d6;
  border-bottom-width: 7px;
  border-radius: 7px 7px 13px 13px;
  background: linear-gradient(90deg, #8e8e8e, #fff, #a5a5a5);
  box-shadow: 0 3px 4px #0003;
}

.id-card {
  position: absolute;
  top: 116px;
  left: 50%;
  width: 190px;
  height: 250px;
  transform: translateX(-50%) rotateX(2deg);
  border-radius: 14px;
  padding: 8px;
  background: linear-gradient(145deg, #fff, #f5e8ef);
  box-shadow:
    0 12px 24px #0003,
    inset 0 0 0 1px #ffffff;
}

.id-inner {
  height: 100%;
  border-radius: 9px;
  border: 1px solid #f2b8d1;
  overflow: hidden;
  background: #fff8fc;
  position: relative;
  text-align: center;
}

.id-header {
  height: 37px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(100deg, #e65391, #ff9ec7);
  color: white;
  font-size: 10px;
  letter-spacing: 2px;
  font-weight: 800;
}

.id-hole {
  position: absolute;
  z-index: 3;
  top: 9px;
  left: 50%;
  transform: translateX(-50%);
  width: 29px;
  height: 6px;
  background: #b43d71;
  border-radius: 20px;
  opacity: .7;
}

.id-photo {
  width: 100px;
  height: 108px;
  margin: 13px auto 8px;
  border-radius: 8px;
  overflow: hidden;
  border: 3px solid white;
  box-shadow: 0 3px 10px #d65c9625;
  background: #ffd8e9;
  display: flex;
  justify-content: center;
  align-items: center;
}

.id-photo img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.id-photo-placeholder {
  color: #b23e73;
  font-size: 30px;
  font-weight: 800;
}

.id-name {
  font-size: 16px;
  color: #30202a;
  font-weight: 800;
  letter-spacing: .5px;
}

.id-role {
  font-size: 9px;
  color: #b34a7c;
  font-weight: 600;
  margin-top: 3px;
}

.id-divider {
  width: 70%;
  height: 1px;
  margin: 10px auto;
  background: #f0bfd5;
}

.id-footer {
  font-size: 8px;
  color: #9a7b8b;
  letter-spacing: 1px;
}

.drag-hint {
  position: absolute;
  top: 340px;
  left: 50%;
  transform: translateX(-50%);
  width: 180px;
  text-align: center;
  color: #a64c78;
  font-size: 9px;
  font-weight: 600;
  letter-spacing: .5px;
  opacity: .85;
}

/* RESPONSIVE */

@media (max-width: 850px) {
  nav {
    padding: 15px 5%;
  }

  .nav-links {
    gap: 13px;
    font-size: 11px;
  }

  .hero {
    gap: 25px;
  }

  .hero-decoration {
    width: 230px;
    height: 300px;
  }

  .project-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .lanyard-stage {
    right: 8px;
    top: 75px;
    transform: scale(.76);
    transform-origin: top right;
  }
}

@media (max-width: 600px) {
  nav {
    padding: 13px 5%;
  }

  .logo {
    font-size: 17px;
  }

  .nav-links {
    gap: 10px;
    font-size: 10px;
  }

  .nav-links a:nth-child(3) {
    display: none;
  }

  section {
    padding: 85px 7%;
  }

  .hero {
    min-height: auto;
    padding-top: 135px;
    padding-bottom: 75px;
    flex-direction: column;
    align-items: flex-start;
  }

  .hero h1 {
    letter-spacing: -2px;
  }

  .hero-decoration {
    align-self: center;
    width: 190px;
    height: 235px;
    margin-top: 10px;
  }

  .hero-monogram {
    font-size: 70px;
  }

  .about-grid {
    grid-template-columns: 1fr;
    gap: 25px;
  }

  .project-grid {
    grid-template-columns: 1fr;
  }

  .project-cover {
    height: 160px;
  }

  .spider-sticky {
    min-height: 90vh;
  }

  .spider-content h2 {
    letter-spacing: -1.5px;
  }

  .lanyard-stage {
    top: 75px;
    right: -9px;
    transform: scale(.61);
    transform-origin: top right;
  }

  .drag-hint {
    display: none;
  }
}

@media (prefers-reduced-motion: reduce) {
  html {
    scroll-behavior: auto;
  }

  * {
    transition-duration: .01ms !important;
  }
}
</style>
</head>

<body>

<nav>
  <a href="#home" class="logo">sarah<span>.</span></a>

  <div class="nav-links">
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#experience">Experience</a>
    <a href="#contact">Contact</a>
  </div>
</nav>

<!-- DRAGGABLE ID CARD -->
<div class="lanyard-stage" id="lanyard" aria-label="Kartu ID yang bisa digerakkan">
  <div class="lanyard-assembly" id="lanyardAssembly">
    <div class="lanyard-ribbon"></div>
    <div class="lanyard-hook"></div>

    <div class="id-card">
      <div class="id-inner">
        <div class="id-hole"></div>
        <div class="id-header">MY PERSONAL ID</div>

        <div class="id-photo">
          <!-- Ganti foto ini dengan foto milikmu -->
          <div class="id-photo-placeholder">S</div>
        </div>

        <div class="id-name">SARAH</div>
        <div class="id-role">SOCIOLOGY STUDENT</div>
        <div class="id-divider"></div>
        <div class="id-footer">CREATIVE MINDS CLUB</div>
      </div>
    </div>
  </div>

  <div class="drag-hint">✦ DRAG ME AROUND ✦</div>
</div>

<!-- HERO -->
<section class="hero" id="home">
  <div class="hero-text">
    <div class="eyebrow">Welcome to my portfolio</div>

    <h1>
      Hi, I'm <span>Sarah.</span><br>
      Creative & Curious.
    </h1>

    <p>
      I'm a Sociology Education student with a multimedia background.
      I enjoy exploring design, digital content, technology, and
      creative business ideas.
    </p>

    <div class="hero-buttons">
      <a href="#projects" class="btn btn-primary">Explore My Work ↗</a>
      <a href="#contact" class="btn btn-outline">Contact Me</a>
    </div>
  </div>

  <div class="hero-decoration">
    <div class="hero-monogram">S.</div>
  </div>
</section>

<!-- ABOUT -->
<section class="about" id="about">
  <div class="section-heading">
    <div class="eyebrow">Get to know me</div>
    <h2>About Me</h2>
    <p>A little introduction about my background and interests.</p>
  </div>

  <div class="about-grid">
    <div class="about-card">
      <div class="big-number">01.</div>
      <h3>Multimedia Background</h3>
      <p>
        I graduated from a vocational high school majoring in
        Multimedia, where I learned computer skills, graphic design,
        video editing, website creation, and digital content production.
      </p>
    </div>

    <div class="about-copy">
      <p>
        I am currently studying Sociology Education at Jakarta State
        University. My academic experience helps me understand people,
        social relationships, and the way society works.
      </p>

      <p>
        I am interested in combining creativity, communication, and
        technology. I also enjoy learning new skills and exploring
        opportunities in digital marketing and business.
      </p>

      <div class="skills">
        <span class="skill">Graphic Design</span>
        <span class="skill">Video Editing</span>
        <span class="skill">HTML & CSS</span>
        <span class="skill">Digital Marketing</span>
        <span class="skill">Content Creation</span>
        <span class="skill">Sociology</span>
      </div>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section class="projects" id="projects">
  <div class="section-heading">
    <div class="eyebrow">Things I've created</div>
    <h2>Selected Projects</h2>
    <p>A collection of creative work and things I have explored.</p>
  </div>

  <div class="project-grid">
    <article class="project-card">
      <div class="project-cover">✿</div>
      <div class="project-info">
        <h3>Graphic Design</h3>
        <p>
          Visual concepts for logos, product packaging, promotional
          materials, and other creative design projects.
        </p>
        <span class="project-type">Design & Branding</span>
      </div>
    </article>

    <article class="project-card">
      <div class="project-cover">▶</div>
      <div class="project-info">
        <h3>Video & Content</h3>
        <p>
          Video editing, product promotion, social media content,
          and digital storytelling.
        </p>
        <span class="project-type">Video Production</span>
      </div>
    </article>

    <article class="project-card">
      <div class="project-cover">⌘</div>
      <div class="project-info">
        <h3>Web & Interactive Media</h3>
        <p>
          Exploring websites, interactive games, simple web
          experiences, and digital projects.
        </p>
        <span class="project-type">Web Development</span>
      </div>
    </article>
  </div>
</section>

<!-- SPIDER-MAN-INSPIRED SCROLL ANIMATION -->
<section class="spider-section" id="creative">
  <div class="spider-sticky">
    <div class="spider-visual">
      <div class="web-lines" id="webLines"></div>
      <div class="spider-orb" id="spiderOrb"></div>
      <div class="spider-symbol" id="spiderSymbol">✳</div>
    </div>

    <div class="spider-content">
      <div class="eyebrow">A little creativity</div>
      <h2>With great ideas<br>comes great creation.</h2>
      <p>
        I believe creativity grows through curiosity, experimentation,
        and the courage to try something new. Every project is a chance
        to learn something different.
      </p>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section class="experience" id="experience">
  <div class="section-heading">
    <div class="eyebrow">My journey</div>
    <h2>Education & Experience</h2>
    <p>The experiences that have helped me grow and develop my skills.</p>
  </div>

  <div class="timeline">
    <div class="timeline-item">
      <div class="date">EDUCATION</div>
      <h3>Universitas Negeri Jakarta</h3>
      <p>
        Sociology Education student, developing an understanding
        of sociology, education, and social life.
      </p>
    </div>

    <div class="timeline-item">
      <div class="date">FEBRUARY 2022 — MAY 2023</div>
      <h3>Content Editor & Digital Marketing Intern</h3>
      <p>
        Worked on product photography, promotional videos, graphic
        design, logo creation, video editing, and digital promotion
        for products and online platforms.
      </p>
    </div>

    <div class="timeline-item">
      <div class="date">CREATIVE EXPERIENCE</div>
      <h3>Multimedia Projects</h3>
      <p>
        Explored graphic design, website creation, interactive games,
        film projects, product packaging, and video animation.
      </p>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section class="contact" id="contact">
  <div class="section-heading">
    <div class="eyebrow">Let's connect</div>
    <h2>Have a project in mind?</h2>
    <p>
      I'm always interested in learning, collaborating, and exploring
      new creative opportunities.
    </p>
  </div>

  <div class="contact-links">
    <!-- Ganti tautan di bawah dengan akunmu -->
    <a class="btn btn-primary"
       href="https://www.linkedin.com/"
       target="_blank" rel="noopener noreferrer">
       LinkedIn ↗
    </a>

    <a class="btn btn-outline"
       href="https://github.com/"
       target="_blank" rel="noopener noreferrer">
       GitHub ↗
    </a>

    <a class="btn btn-outline"
       href="mailto:your-email@example.com">
       Email Me ↗
    </a>
  </div>
</section>

<footer>
  © 2026 Sarah. Made with creativity and curiosity ♡
</footer>

<script>
/* ==========================================
   DRAGGABLE LANYARD
   Mouse + touchscreen support
========================================== */

const lanyard = document.getElementById("lanyard");
const assembly = document.getElementById("lanyardAssembly");

let dragging = false;
let startPointerX = 0;
let startPointerY = 0;
let initialX = 0;
let initialY = 0;
let currentX = 0;
let currentY = 0;
let currentTilt = 0;
let previousPointerX = 0;
let velocityX = 0;

function updateLanyard() {
  assembly.style.setProperty("--lanyard-x", currentX + "px");
  assembly.style.setProperty("--lanyard-y", currentY + "px");
  assembly.style.setProperty("--lanyard-tilt", currentTilt + "deg");
}

lanyard.addEventListener("pointerdown", function(event) {
  dragging = true;

  startPointerX = event.clientX;
  startPointerY = event.clientY;

  initialX = currentX;
  initialY = currentY;

  previousPointerX = event.clientX;
  velocityX = 0;

  lanyard.setPointerCapture(event.pointerId);
});

lanyard.addEventListener("pointermove", function(event) {
  if (!dragging) return;

  const dx = event.clientX - startPointerX;
  const dy = event.clientY - startPointerY;

  currentX = initialX + dx;
  currentY = initialY + dy;

  velocityX = event.clientX - previousPointerX;
  previousPointerX = event.clientX;

  currentTilt = Math.max(-28, Math.min(28, velocityX * 1.3));

  updateLanyard();
});

function stopDragging() {
  if (!dragging) return;

  dragging = false;

  const settle = () => {
    if (dragging) return;

    currentTilt *= 0.88;

    if (Math.abs(currentTilt) < 0.15) {
      currentTilt = 0;
      updateLanyard();
      return;
    }

    updateLanyard();
    requestAnimationFrame(settle);
  };

  requestAnimationFrame(settle);
}

lanyard.addEventListener("pointerup", stopDragging);
lanyard.addEventListener("pointercancel", stopDragging);
lanyard.addEventListener("lostpointercapture", stopDragging);

/* ==========================================
   SCROLL ANIMATION
   Spider-inspired visual grows while scrolling
========================================== */

const spiderSection = document.querySelector(".spider-section");
const spiderOrb = document.getElementById("spiderOrb");
const webLines = document.getElementById("webLines");
const spiderSymbol = document.getElementById("spiderSymbol");

function updateScrollAnimation() {
  const rect = spiderSection.getBoundingClientRect();
  const viewportHeight = window.innerHeight;

  const totalDistance = rect.height + viewportHeight;
  const traveled = viewportHeight - rect.top;

  let progress = traveled / totalDistance;
  progress = Math.max(0, Math.min(1, progress));

  const scale = 0.35 + progress * 1.15;
  const rotation = progress * 35;

  spiderOrb.style.transform =
    `translate(-50%, -50%) scale(${scale})`;

  webLines.style.transform =
    `rotate(${rotation}deg) scale(${1 + progress * 0.25})`;

  spiderSymbol.style.transform =
    `translate(-50%, -50%) rotate(${progress * 180}deg) scale(${0.6 + progress * 0.8})`;
}

window.addEventListener("scroll", updateScrollAnimation, {
  passive: true
});

window.addEventListener("resize", updateScrollAnimation);

updateLanyard();
updateScrollAnimation();
</script>

</body>
</html>