<template>
  <div id="app">
    <div id="nav">
      <div class="nav-image">
        <router-link to="/">
          <img src="./assets/mohsenlogo.png" alt=""
        /></router-link>
      </div>
      <div class="nav-links" routerLinkActive="active_route">
        <router-link class="nav-link" to="/">Startseite</router-link>
        <router-link class="nav-link" to="/services">Services</router-link>
        <router-link class="nav-link" to="/about">Uber Mich</router-link>
        <router-link class="nav-link" to="/contact">Kontakt</router-link>
      </div>
      <div class="footer-links">
        <div class="privacy-links">
          <router-link class="footer-link" to="/privacy">Impressum</router-link>
          <router-link class="footer-link" to="privacy"
            >Datenschutz</router-link
          >
        </div>

        <a href="paradisestudio.de"
          ><div class="copyright-text">
            <p>c. 2021</p>
            <p>Paradise Studio</p>
          </div>
        </a>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap");

* {
  margin: 0;
}

#app {
  display: flex;
  scroll-behavior: smooth;
}

#nav {
  display: flex;
  position: fixed;
  z-index: 1000;
  flex-direction: column;
  width: 125px;
  border-right: 1px solid lightgray;
  height: 100vh;
  font-family: "Fjalla One", sans-serif;
  text-align: center;
  -webkit-animation: fade-in 1s cubic-bezier(0.39, 0.575, 0.565, 1) 1.5s both;
  animation: fade-in 1s cubic-bezier(0.39, 0.575, 0.565, 1) 1.5s both;
}

@-webkit-keyframes fade-in {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@keyframes fade-in {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

#nav img {
  width: 125px;
  border-bottom: 1px solid lightgray;
}

.nav-links {
  display: flex;
  flex-direction: column;
  height: 100vh;
  justify-content: space-evenly;
  align-items: center;
}

.nav-link {
  text-decoration: none;
  color: black;
  text-transform: uppercase;
  font-size: 18px;
}

.nav-link:hover {
  text-decoration: underline;
}

.router-link-exact-active {
  text-decoration: underline;
}

.footer-link,
a {
  text-decoration: none;
  color: black;
  text-transform: uppercase;
  font-size: 12px;
}

.footer-link {
  margin-bottom: 1rem;
}

.footer-links {
  display: flex;
  flex-direction: column;
}

.privacy-links {
  display: flex;
  flex-direction: column;
  line-height: 0;
}

.copyright-text {
  font-size: 10px;
  text-align: center;
}

@media only screen and (max-width: 800px) {
}

@media only screen and (max-width: 600px) {
}

@media only screen and (max-width: 375px) {
  #nav {
    display: flex;
    flex-direction: column;
    width: 100px;
  }

  #nav img {
    width: 100px;
  }
}
</style>
