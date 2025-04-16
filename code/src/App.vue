<script setup>
function scrollToSection(id) {
  const section = document.getElementById(id);
  if (section) {
    section.scrollIntoView({ behavior: "smooth" });
  }
}
</script>

<template>
  <header>
    <nav class="navbar">
      <div class="logo">
        <img src="./assets/images/icons/logo.svg" alt="Sunnyside Logo" />
      </div>
      <ul class="nav-links">
        <li>
          <a @click.prevent="scrollToSection('about')">About</a>
        </li>
        <li>
          <a @click.prevent="scrollToSection('services')">Services</a>
        </li>
        <li>
          <a @click.prevent="scrollToSection('projects')">Projects</a>
        </li>
        <li><button @click="scrollToSection('contacts')">CONTACT</button></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-overlay">
      <h1 class="hero-title">WE ARE CREATIVES</h1>
      <img
        src="./assets/images/icons/icon-arrow-down.svg"
        class="arrow-down"
        alt="Arrow Down"
      />
    </div>
    <picture class="hero-image">
      <source
        media="(min-width: 1024px)"
        srcset="./assets/images/desktop/image-header.jpg"
      />
      <source
        media="(max-width: 768px)"
        srcset="./assets/images/mobile/image-header.jpg"
      />
      <img
        src="./assets/images/mobile/image-header.jpg"
        class="hero-image"
        alt="Hero Image"
      />
    </picture>
  </section>

  <section id="about" class="about">
    <div class="transform-message">
      <h2>Transform your brand</h2>
      <p>
        We are a full-service creative agency specializing in helping brands
        grow fast. Engage your clients through compelling visuals that do most
        of the marketing for you.
      </p>
      <button>LEARN MORE</button>
    </div>
    <picture class="transform-image">
      <source
        media="(min-width: 1024px)"
        srcset="./assets/images/desktop/image-transform.jpg"
      />
      <source
        media="(max-width: 768px)"
        srcset="./assets/images/mobile/image-transform.jpg"
      />
      <img
        src="./assets/images/mobile/image-transform.jpg"
        class="transform-image"
        alt="Transform Image"
      />
    </picture>
    <picture class="standout-image">
      <source
        media="(min-width: 1024px)"
        srcset="./assets/images/desktop/image-stand-out.jpg"
      />
      <source
        media="(max-width: 768px)"
        srcset="./assets/images/mobile/image-stand-out.jpg"
      />
      <img
        src="./assets/images/mobile/image-stand-out.jpg"
        class="standout-image"
        alt="Stand Out Image"
      />
    </picture>
    <div class="standout-message">
      <h2>Stand out to the right audience</h2>
      <p>
        Using a collaborative formula of designers, researchers, photographers,
        videographers, and copywriters, we'll build and extend your brand in
        digital places.
      </p>
      <button>LEARN MORE</button>
    </div>
  </section>

  <section id="services" class="services">
    <div class="graphic-service">
      <picture class="graphic-image">
        <source
          media="(min-width: 1024px)"
          srcset="./assets/images/desktop/image-graphic-design.jpg"
        />
        <source
          media="(max-width: 768px)"
          srcset="./assets/images/mobile/image-graphic-design.jpg"
        />
        <img
          src="./assets/images/mobile/image-graphic-design.jpg"
          class="graphic-image"
          alt="Graphic Design Service"
        />
      </picture>
      <div class="graphic-message">
        <h2>Graphic Design</h2>
        <p>
          Great design makes you memorable. We deliver artwork that underscores
          your brand message and captures potential clients' attention.
        </p>
      </div>
    </div>
    <div class="photography-service">
      <picture class="photography-image">
        <source
          media="(min-width: 1024px)"
          srcset="./assets/images/desktop/image-photography.jpg"
        />
        <source
          media="(max-width: 768px)"
          srcset="./assets/images/mobile/image-photography.jpg"
        />
        <img
          src="./assets/images/mobile/image-photography.jpg"
          class="photography-image"
          alt="Photography Service"
        />
      </picture>
      <div class="photography-message">
        <h2>Photography</h2>
        <p>
          Increase your credibility by getting the most stunning, high-quality
          photos that improve your business image.
        </p>
      </div>
    </div>
  </section>

  <section id="projects" class="testimonials">
    <h2>CLIENT TESTIMONIALS</h2>
    <div class="clients-testimonials">
      <div class="client">
        <img
          src="./assets/images/profiles/image-emily.jpg"
          alt="Emily R."
          class="client-image"
        />
        <p>
          We put our trust in Sunnyside and they delivered, making sure our
          needs were met and deadlines were always hit.
        </p>
        <h3>Emily R.</h3>
        <h4>Marketing Director</h4>
      </div>
      <div class="client">
        <img
          src="./assets/images/profiles/image-thomas.jpg"
          alt="Thomas S."
          class="client-image"
        />
        <p>
          Sunnyside's enthusiasm coupled with their keen interest in our brand's
          success made it a satisfying and enjoyable experience.
        </p>
        <h3>Thomas S.</h3>
        <h4>Chief Operating Officer</h4>
      </div>
      <div class="client">
        <img
          src="./assets/images/profiles/image-jennie.jpg"
          alt="Jennie F."
          class="client-image"
        />
        <p>
          Incredible end result! Our sales increased over 400% when we worked
          with Sunnyside. Highly recommended!
        </p>
        <h3>Jennie F.</h3>
        <h4>Business Owner</h4>
      </div>
    </div>
  </section>

  <section class="gallery">
    <picture class="gallery-item">
      <source
        media="(min-width: 1024px)"
        srcset="./assets/images/desktop/image-gallery-milkbottles.jpg"
      />
      <source
        media="(max-width: 768px)"
        srcset="./assets/images/mobile/image-gallery-milkbottles.jpg"
      />
      <img
        src="./assets/images/mobile/image-gallery-milkbottles.jpg"
        alt="Gallery Milk Bottles"
      />
    </picture>
    <picture class="gallery-item">
      <source
        media="(min-width: 1024px)"
        srcset="./assets/images/desktop/image-gallery-orange.jpg"
      />
      <source
        media="(max-width: 768px)"
        srcset="./assets/images/mobile/image-gallery-orange.jpg"
      />
      <img
        src="./assets/images/mobile/image-gallery-orange.jpg"
        alt="Gallery Orange"
      />
    </picture>
    <picture class="gallery-item">
      <source
        media="(min-width: 1024px)"
        srcset="./assets/images/desktop/image-gallery-cone.jpg"
      />
      <source
        media="(max-width: 768px)"
        srcset="./assets/images/mobile/image-gallery-cone.jpg"
      />
      <img
        src="./assets/images/mobile/image-gallery-cone.jpg"
        alt="Gallery Cone"
      />
    </picture>
    <picture class="gallery-item">
      <source
        media="(min-width: 1024px)"
        srcset="./assets/images/desktop/image-gallery-sugarcubes.jpg"
      />
      <source
        media="(max-width: 768px)"
        srcset="./assets/images/mobile/image-gallery-sugarcubes.jpg"
      />
      <img
        src="./assets/images/mobile/image-gallery-sugarcubes.jpg"
        alt="Gallery Sugar Cubes"
      />
    </picture>
  </section>

  <footer id="contacts">
    <img
      src="./assets/images/icons/logo-green.svg"
      class="footer-logo"
      alt="Sunnyside logo"
    />

    <div class="footer-nav">
      <ul class="footer-nav-links">
        <li>
          <a @click.prevent="scrollToSection('about')">About</a>
        </li>
        <li>
          <a @click.prevent="scrollToSection('services')">Services</a>
        </li>
        <li>
          <a @click.prevent="scrollToSection('projects')">Projects</a>
        </li>
      </ul>
    </div>

    <div class="footer-socials">
      <img src="./assets/images/icons/icon-facebook.svg" alt="Facebook" />
      <img src="./assets/images/icons/icon-instagram.svg" alt="Instagram" />
      <img src="./assets/images/icons/icon-twitter.svg" alt="Twitter / X" />
      <img src="./assets/images/icons/icon-pinterest.svg" alt="Pinterest" />
    </div>
  </footer>
</template>

<style scoped>
/* ----- HEADER ----- */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2.5rem;
  position: absolute;
  top: 0;
  left: 0;
  width: -webkit-fill-available;
  width: -moz-available;
  z-index: 1;
}

.nav-links {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 3rem;
  list-style: none;
}

.nav-links li a {
  text-decoration: none;
  color: hsl(0, 0%, 100%);
  cursor: pointer;
}

.nav-links li button {
  font-family: "Fraunces";
  background-color: hsl(0, 0%, 100%);
  color: hsl(0, 0%, 0%);
  height: 3rem;
  padding: 1.8rem 2.3rem;
  border: none;
  border-radius: 30px;
  display: flex;
  align-items: center;
  cursor: pointer;
}

.nav-links li button:hover {
  background-color: hsl(0, 0%, 100%, 30%);
  color: hsl(0, 0%, 100%);
}

/* ----- HERO SECTION ----- */
.hero {
  position: relative;
  overflow: hidden;
}

.hero-overlay {
  display: flex;
  flex-direction: column;
  position: absolute;
  align-items: center;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: hsl(0, 0%, 100%);
  gap: 7vh;
  width: max-content;
  z-index: 2;
}

.hero-title {
  font-family: "Fraunces";
  font-size: 3rem;
  font-weight: 900;
  letter-spacing: 0.5rem;
  text-align: center;
}

.arrow-down {
  width: 2rem;
}

.hero-image {
  width: 100%;
  height: auto;
  display: block;
  object-fit: cover;
}

/* ----- ABOUT SECTION ----- */
.about {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

.transform-message,
.standout-message {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  width: 100%;
  padding: 0 16%;
  resize: none;
  box-sizing: border-box;
}

.transform-message h2,
.standout-message h2 {
  font-family: "Fraunces";
  font-size: 2.8rem;
  font-weight: 900;
  color: hsl(0, 0%, 0%);
}

.transform-message p,
.standout-message p {
  font-size: 1.2rem;
  color: hsl(232, 10%, 55%);
  line-height: 1.5;
}

.transform-message button,
.standout-message button {
  font-family: "Fraunces";
  font-weight: 900;
  background-color: transparent;
  color: hsl(0, 0%, 0%);
  border: none;
  position: relative;
  display: flex;
  align-items: center;
  margin-top: 2vh;
  padding: 0;
  cursor: pointer;
  width: 30%;
  height: fit-content;
  justify-content: center;
}

.transform-message button::after,
.standout-message button::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -2px;
  width: 100%;
  height: 10px;
  z-index: -1;
  border-radius: 10px;
}

.transform-message button::after {
  background-color: hsl(51, 100%, 49%, 25%);
}

.transform-message button:hover::after {
  background-color: hsl(51, 100%, 49%);
}

.standout-message button::after {
  background-color: hsl(7, 99%, 70%, 25%);
}

.standout-message button:hover::after {
  background-color: hsl(7, 99%, 70%);
}

.transform-image,
.standout-image {
  width: 100%;
  height: auto;
  display: block;
  object-fit: cover;
}

/* ----- SERVICES SECTION ----- */
.services {
  display: flex;
  flex-direction: row;
}

.graphic-service,
.photography-service {
  position: relative;
  width: 50%;
}

.graphic-message,
.photography-message {
  position: absolute;
  bottom: 5%;
  left: 50%;
  transform: translateX(-50%);
  text-align: center;
  width: 100%;
  padding: 0 22%;
  resize: none;
  box-sizing: border-box;
}

.graphic-message h2,
.photography-message h2 {
  font-family: "Fraunces";
  font-size: 2rem;
  font-weight: 900;
}

.graphic-message p,
.photography-message p {
  font-size: 1.2rem;
  line-height: 1.5;
}

.graphic-message {
  color: hsl(167, 40%, 24%);
}

.photography-message {
  color: hsl(198, 62%, 26%);
}

.graphic-image,
.photography-image {
  width: 100%;
  height: auto;
  display: block;
  object-fit: cover;
}

/* ----- TESTIMONIALS SECTION ----- */
.testimonials {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 10rem;
}

.testimonials h2 {
  font-family: "Fraunces";
  font-size: 1.2rem;
  font-weight: 900;
  color: hsl(210, 4%, 67%);
  margin-bottom: 5rem;
  letter-spacing: 0.3rem;
}

.clients-testimonials {
  display: flex;
  flex-direction: row;
  gap: 3rem;
}

.client {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width: 33%;
}

.client-image {
  width: 75px;
  border-radius: 50%;
  margin-bottom: 2rem;
}

.client p {
  color: hsl(213, 9%, 39%);
  font-size: 1.1rem;
  line-height: 1.7;
}

.client h3 {
  font-family: "Fraunces";
  font-size: 1.1rem;
  font-weight: 900;
  margin: 3rem 0 0;
}

.client h4 {
  font-size: 0.9rem;
  color: hsl(210, 4%, 67%);
  margin-top: 0.8rem;
}

/* ----- GALLERY SECTION ----- */
.gallery {
  display: flex;
  flex-direction: row;
}

.gallery-item img {
  width: 100%;
  height: auto;
  display: block;
  object-fit: cover;
}

/* ----- FOOTER ----- */
footer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 3rem;
  color: hsl(168, 34%, 41%);
  background-color: hsl(168, 40%, 70%);
}

.footer-logo {
  width: 10rem;
  margin: 1.5rem;
}

.footer-nav {
  margin-bottom: 4rem;
}

.footer-nav-links {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 3.5rem;
  list-style: none;
  padding: 0;
}

.footer-nav-links li a {
  text-decoration: none;
  color: hsl(168, 34%, 41%);
  font-size: 1.2rem;
  cursor: pointer;
}

.footer-nav-links li a:hover {
  color: hsl(0, 0%, 100%);
}

.footer-socials {
  display: flex;
  gap: 2rem;
  margin-bottom: 1.5rem;
}

.footer-socials img {
  cursor: pointer;
}

.footer-socials img:hover {
  filter: brightness(0) invert(1);
}
</style>
