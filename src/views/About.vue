<template>
  <div>
    <div class="logo-image">
      <img src="../assets/mologogreen.jpg" alt="" />
    </div>
    <div class="about">
      <div class="about-image">
        <img src="../assets/mohsenbio.png" alt="" />
      </div>
      <div class="about-text">
        <h2>uber mich</h2>
        <h1>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatibus
          rem sit deserunt dignissimos porro sed dolore placeat assumenda, enim
          hic! Nihil blanditiis animi inventore dolor asperiores ab beatae nobis
          deserunt perferendis reprehenderit?
        </h1>
        <h1>
          Consectetur ex optio harum voluptas minima quam possimus corporis rem
          mollitia explicabo adipisci nulla, aliquam natus cum, cumque ipsam
          quis vel enim maxime, velit sapiente! Aliquam pariatur ad officiis
          neque excepturi esse natus nostrum eligendi quisquam voluptate quas
          qui a maiores odit sint, ea iure?
        </h1>
        <h1>
          Dolorum, at voluptatum pariatur voluptas est quisquam facere amet
          labore laborum nulla dolorem architecto nobis culpa accusamus. Veniam
          facilis magni quae nostrum quia!
        </h1>
        <router-link class="learn-more" to="/contact">kontakt mich</router-link>
      </div>
    </div>
  </div>
</template>

<style scoped>
.logo-image {
  position: fixed;
  right: 0;
  z-index: 1;
  -webkit-animation: slide-in-left 1s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
  animation: slide-in-left 1s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
}

@-webkit-keyframes slide-in-left {
  0% {
    -webkit-transform: translateX(-1000px);
    transform: translateX(-1000px);
    opacity: 0;
  }
  100% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
    opacity: 50;
  }
}
@keyframes slide-in-left {
  0% {
    -webkit-transform: translateX(-1000px);
    transform: translateX(-1000px);
    opacity: 0;
  }
  100% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
    opacity: 50;
  }
}

.logo-image img {
  height: 100vh;
  filter: blur(5px);
  -webkit-filter: blur(5px);
}

.about {
  -webkit-animation: fade-in 0.5s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
  animation: fade-in 0.5s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
  z-index: 2;
  position: fixed;
  display: flex;
  width: 100%;
  height: 100%;
  align-items: center;
  margin-left: 10rem;
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

.about-image img {
  width: 400px;
}

.about-text {
  width: 500px;
  margin-left: 3rem;
}

h1 {
  font-family: "Roboto", sans-serif;
  font-size: 18px;
  line-height: 2rem;
  margin-bottom: 1rem;
}

h2 {
  font-family: "Fjalla One", sans-serif;
  margin-bottom: 1rem;
  font-size: 16px;
}

.learn-more {
  font-size: 16px;
  font-weight: bold;
  text-decoration: underline;
  font-family: "Roboto", sans-serif;
}

@media only screen and (max-width: 800px) {
  .services {
    margin-left: 3rem;
  }
  h1 {
    font-family: "Roboto", sans-serif;
    font-size: 12px;
    line-height: 1rem;
  }

  h2 {
    font-family: "Fjalla One", sans-serif;
    margin-bottom: 0.5rem;
    font-size: 12px;
  }

  .logo-image img {
    height: 50vh;
  }

  .logo-image {
    position: fixed;
    top: 50%;
    z-index: 2;
  }

  .about {
    flex-direction: column;
  }

  .about-image {
    margin-top: 1rem;
  }

  .about-image img {
    width: 200px;
  }

  .about-text {
    width: 250px;
    margin-left: 0;
    margin-right: 1rem;
    margin-top: 2rem;
  }
}
</style>
