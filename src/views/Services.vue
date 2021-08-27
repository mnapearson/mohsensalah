<template>
  <div>
    <div class="logo-image">
      <img src="../assets/mologogray.jpg" alt="" />
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
      <div class="service-two">
        <div class="service-two-text">
          <h2>service two</h2>
          <h1>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sunt,
            minus delectus! Recusandae deleniti nulla, et dolores eaque magnam
            repellat odio.
          </h1>
        </div>
        <div class="service-two-image">
          <img src="../assets/servicetwo.png" alt="" />
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
  display: flex;
  position: fixed;
  flex-direction: column;
  margin-left: 4rem;
  justify-content: center;
  width: 100%;
  height: 100%;
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

.service-one {
  z-index: 2;
  display: flex;
  align-items: center;
}

.service-two {
  z-index: 2;
  display: flex;
  align-items: center;
  margin-top: 2rem;
}

.service-one-text {
  width: 400px;
  margin: 3rem;
}

.service-two-text {
  width: 300px;
  margin: 3rem;
}

h1 {
  font-family: "Roboto", sans-serif;
  font-size: 18px;
  line-height: 2rem;
}

h2 {
  font-family: "Fjalla One", sans-serif;
  margin-bottom: 1rem;
  font-size: 16px;
}

.service-one img {
  height: 400px;
}

.service-two img {
  height: 300px;
}

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
    opacity: 1;
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
    opacity: 1;
  }
}

.logo-image img {
  height: 100vh;
  opacity: 50%;
  filter: blur(5px);
  -webkit-filter: blur(5px);
}

.logo-image img {
  height: 100vh;
  opacity: 50%;
  filter: blur(5px);
  -webkit-filter: blur(5px);
}
</style>
