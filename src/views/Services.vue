<template>
  <div>
    <div class="logo-image">
      <img src="../assets/mologoblack.jpg" alt="" />
    </div>
    <div class="services">
      <div class="service-one">
        <div class="service-one-image">
          <img src="../assets/serviceone.png" alt="" />
        </div>
        <div class="service-one-text">
          <h2>service one</h2>
          <h1>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sunt,
            minus delectus! Recusandae deleniti nulla, et dolores eaque magnam
            repellat odio.
          </h1>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.services {
  -webkit-animation: fade-in 0.5s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
  animation: fade-in 0.5s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
  z-index: 2;
  position: fixed;
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

.logo-image {
  position: fixed;
  z-index: 1;
  -webkit-animation: slide-in-right 1s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
  animation: slide-in-right 1s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
}

.service-one {
  z-index: 2;
  position: fixed;
  display: flex;
  align-items: center;
  top: 10%;
  left: 20%;
}

.service-one-text {
  width: 40%;
  margin: 3rem;
}

h1 {
  font-family: "Roboto", sans-serif;
  font-size: 18px;
  line-height: 2rem;
}

h2 {
  font-family: "Fjalla One", sans-serif;
}

.service-one img {
  height: 400px;
}

@-webkit-keyframes slide-in-right {
  0% {
    -webkit-transform: translateX(1000px);
    transform: translateX(1000px);
    opacity: 0;
  }
  100% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
    opacity: 1;
  }
}
@keyframes slide-in-right {
  0% {
    -webkit-transform: translateX(1000px);
    transform: translateX(1000px);
    opacity: 0;
  }
  100% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
    opacity: 1;
  }
}

.logo-image img {
  -webkit-transform: scaleX(-1);
  transform: scaleX(-1);
  height: 100vh;
  opacity: 50%;
  filter: blur(5px);
  -webkit-filter: blur(5px);
}
</style>
