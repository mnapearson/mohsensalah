<template>
  <div id="app">
    <div id="nav">
      <div class="nav-image">
        <img src="./assets/mohsenlogo.png" alt="" />
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
            <p>copyright 2021</p>
            <p>🌴 Paradise Studio</p>
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
}

#nav {
  display: flex;
  flex-direction: column;
  width: 150px;
  border-right: 1px solid lightgray;
  height: 100vh;
  font-family: "Fjalla One", sans-serif;
  text-align: center;
  -webkit-animation: swing-in-left-bck 1s
    cubic-bezier(0.175, 0.885, 0.32, 1.275) 3s both;
  animation: swing-in-left-bck 1s cubic-bezier(0.175, 0.885, 0.32, 1.275) 3s
    both;
}

@-webkit-keyframes swing-in-left-bck {
  0% {
    -webkit-transform: rotateY(-70deg);
    transform: rotateY(-70deg);
    -webkit-transform-origin: left;
    transform-origin: left;
    opacity: 0;
  }
  100% {
    -webkit-transform: rotateY(0);
    transform: rotateY(0);
    -webkit-transform-origin: left;
    transform-origin: left;
    opacity: 1;
  }
}
@keyframes swing-in-left-bck {
  0% {
    -webkit-transform: rotateY(-70deg);
    transform: rotateY(-70deg);
    -webkit-transform-origin: left;
    transform-origin: left;
    opacity: 0;
  }
  100% {
    -webkit-transform: rotateY(0);
    transform: rotateY(0);
    -webkit-transform-origin: left;
    transform-origin: left;
    opacity: 1;
  }
}

#nav img {
  width: 150px;
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
  font-size: 25px;
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
}

.copyright-text {
  font-size: 12px;
  text-align: center;
}
</style>
