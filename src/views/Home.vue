<template>
  <div class="home">
    <div>
      <div class="text">
        <h2>wilkkomen bei projekt koerper therapie</h2>
        <h1>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Earum amet
          magnam iusto quia, ex dolores, commodi eveniet sed repellendus natus
          quibusdam voluptatibus laboriosam voluptates quis doloribus
          consequuntur. Alias, sint. Eius consequatur, distinctio fuga
          doloremque praesentium sed quas. Beatae magni molestiae numquam.
          Veritatis consequuntur voluptatum earum ut eius quod reiciendis
          impedit veniam odio.
        </h1>
        <h1>
          Iste fuga quaerat accusantium et! Molestias deserunt, commodi velit
          neque sed odit porro. Nesciunt sapiente nihil soluta, laudantium
          temporibus dignissimos possimus!
        </h1>
        <h1>
          Aspernatur quidem vel, necessitatibus porro consectetur dolorum vitae
          voluptas repellendus, cumque consequuntur facilis, aperiam praesentium
          blanditiis omnis quaerat?
        </h1>
        <router-link class="learn-more" to="/services">learn more</router-link>
      </div>
    </div>
    <div class="image">
      <img class="image-1" src="../assets/mologoblack.jpg" alt="" />
      <img class="image-2" src="../assets/mologogray.jpg" alt="" />
      <img class="image-3" src="../assets/mologogreen.jpg" alt="" />
    </div>
    <div class="logo"><img src="../assets/mohsenlogo.png" alt="" /></div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap");
.home {
  display: flex;
  justify-content: center;
  align-items: center;
}

h2 {
  font-family: "Fjalla One", sans-serif;
  margin-bottom: 1rem;
  font-size: 16px;
}

.text {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: left;
  font-family: "Roboto", sans-serif;
  font-size: 10px;
  width: 40%;
  padding: 6rem;
  line-height: 2rem;
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

h1 {
  margin-bottom: 2rem;
}

.image {
  -webkit-animation: fade-out 1s ease-out 1.8s both;
  animation: fade-out 1s ease-out 1.8s both;
}

@-webkit-keyframes fade-out {
  0% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}
@keyframes fade-out {
  0% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}

.image-1 {
  position: fixed;
  top: 5%;
  right: 15%;
}

.image-2 {
  position: fixed;
  top: 35%;
  right: 15%;
}

.image-3 {
  position: fixed;
  top: 65%;
  right: 15%;
}

.image img {
  height: 30vh;
}

.image-1 {
  -webkit-animation: slide-in-left 1.5s cubic-bezier(0.25, 0.46, 0.45, 0.94)
    both;
  animation: slide-in-left 1.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;
}

.image-2 {
  -webkit-animation: slide-in-left 1.5s cubic-bezier(0.25, 0.46, 0.45, 0.94)
    0.5s both;
  animation: slide-in-left 1.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) 0.5s both;
}

.image-3 {
  -webkit-animation: slide-in-left 1.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) 1s
    both;
  animation: slide-in-left 1.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) 1s both;
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

.learn-more {
  font-size: 16px;
  font-weight: bold;
  text-decoration: underline;
}

.logo {
  position: fixed;
  top: 0;
  right: 0;
  -webkit-animation: fade-in 1s cubic-bezier(0.39, 0.575, 0.565, 1) 3s both;
  animation: fade-in 1s cubic-bezier(0.39, 0.575, 0.565, 1) 3s both;
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

.logo img {
  height: 100vh;
  width: auto;
}
</style>
