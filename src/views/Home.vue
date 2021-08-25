<template>
  <div class="home">
    <div>
      <div class="text">
        <h1>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Earum amet
          magnam iusto quia, ex dolores, commodi eveniet sed repellendus natus
          quibusdam voluptatibus laboriosam voluptates quis doloribus
          consequuntur. Alias, sint. Sunt velit similique, fuga est praesentium
          maxime! Eius consequatur, distinctio fuga doloremque praesentium sed
          quas. Beatae magni molestiae numquam. Veritatis consequuntur
          voluptatum earum ut eius quod reiciendis impedit veniam odio.
        </h1>
        <h1>
          Iste fuga quaerat accusantium et! Molestias deserunt, commodi velit
          neque sed odit porro. Dicta amet quas vitae necessitatibus voluptate
          veniam error maxime perspiciatis incidunt at fuga vero aliquid placeat
          qui deleniti est et rerum odit porro, aut sapiente. Sapiente labore
          vitae officia asperiores praesentium. Nemo quos nulla fuga laudantium
          optio, accusantium eveniet commodi earum ducimus, reprehenderit
          impedit beatae explicabo sed architecto at exercitationem iusto
          libero!
        </h1>
        <h1>
          Nesciunt sapiente nihil soluta, laudantium temporibus dignissimos
          possimus! Aspernatur quidem vel, necessitatibus porro consectetur
          dolorum vitae voluptas repellendus, cumque consequuntur facilis,
          aperiam praesentium blanditiis omnis quaerat?
        </h1>
      </div>
    </div>
    <div class="image">
      <img src="../assets/bordershadowlogo.png" alt="" />
    </div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap");
.home {
  display: flex;
}

.text {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-family: "Roboto", sans-serif;
  font-size: 10px;
  width: 40%;
  padding: 6rem 0 6rem 6rem;
  line-height: 2rem;
  -webkit-animation: fade-in 1s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
  animation: fade-in 1s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
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
</style>
