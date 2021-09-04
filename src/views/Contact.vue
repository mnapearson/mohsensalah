<template>
  <div>
    <div class="logo-image">
      <img src="../assets/mologoblack.jpg" alt="" />
    </div>
    <div class="contact">
      <div class="contact-main">
        <h1>kontakt</h1>
        <div class="contact-form">
          <form
            ref="contact"
            class="contact-form"
            @submit.prevent="sendEmail"
            v-if="!successMessage"
          >
            <input type="text" name="user_name" placeholder="name" />

            <input type="email" name="user_email" placeholder="email" />

            <textarea
              name="message"
              placeholder="message"
              type="message"
            ></textarea>
            <input type="submit" value="Send" />
          </form>
          <p v-if="successMessage">
            Thank you for your message. <br />You will receive a reply as soon
            as possible.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import emailjs from "emailjs-com";

export default {
  data() {
    return {
      name: "",
      email: "",
      message: "",
      successMessage: false,
    };
  },
  methods: {
    sendEmail(e) {
      try {
        emailjs.sendForm(
          "service_9kxr7d6",
          "template_yffeype",
          e.target,
          "user_o6tM95YAVRykwYE7z90AI",
          {
            name: this.name,
            email: this.email,
            message: this.message,
          }
        );
      } catch (error) {
        console.log({ error });
      }
      // Reset form field
      this.name = "";
      this.email = "";
      this.message = "";
      this.successMessage = true;
    },
  },
};
</script>

<style scoped>
.contact {
  -webkit-animation: fade-in 0.5s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
  animation: fade-in 0.5s cubic-bezier(0.39, 0.575, 0.565, 1) 1s both;
  z-index: 2;
  display: flex;
  position: fixed;
  flex-direction: column;
  margin-left: 10rem;
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

h1 {
  font-family: "Fjalla One", sans-serif;
  margin-bottom: 1rem;
  font-size: 16px;
}

.contact-form {
  text-align: center;
  font-size: 12px;
  line-height: 22px;
  width: 500px;
}

label {
  float: left;
}

input[type="text"],
[type="email"],
textarea {
  width: 100%;
  padding: 12px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
}

input[type="submit"] {
  padding: 12px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

textarea {
  height: 200px;
}

input[type="submit"]:hover {
  background: black;
  color: white;
}

.success {
  position: fixed;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.logo-image {
  position: fixed;
  right: 0;
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

@media only screen and (max-width: 800px) {
  h1 {
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

  .contact-form {
    text-align: center;
    font-size: 12px;
    line-height: 22px;
    width: 250px;
  }

  .contact {
    margin-left: 8rem;
  }
}
</style>
