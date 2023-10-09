<script>
import { Clipboard } from "v-clipboard";

export default {
  name: "App",
  data() {
    return {
      isCopied: true,
    };
  },
  methods: {
    // success() {
    //   alert("success");
    // },
    // copy() {
    //   Clipboard.copy("TEST");
    // },
    ToggleCopied() {
      this.isCopied = !this.isCopied;
    },
  },
};
</script>

<template>
  <div class="totalite" id="contact">
    <div class="titre">
      <h3>CONTACT</h3>
    </div>
    <div class="login-card-container">
      <form
        action="https://formcarry.com/s/DPW3iJbBnC"
        method="POST"
        accept-charset="UTF-8"
        class="login-card-form"
      >
        <div class="login-card-form-2">
          <div class="form-item">
            <span class="form-item-icon material-symbols-rounded">person</span>
            <input
              type="text"
              placeholder="Nom"
              id="nom"
              name="lastName"
              required
            />
          </div>
          <div class="form-item">
            <span class="form-item-icon material-symbols-rounded">person</span>
            <input
              type="text"
              placeholder="Prénom"
              id="prenom"
              name="firstName"
              required
            />
          </div>
        </div>

        <div class="form-item">
          <span class="form-item-icon material-symbols-rounded">mail</span>
          <input
            type="email"
            placeholder="Email"
            id="email"
            name="email"
            required
          />
        </div>
        <input type="hidden" name="_gotcha" />
        <div class="form-item">
          <textarea id="message" name="message" required></textarea>
        </div>
        <button type="submit" class="btn">Envoyer</button>
      </form>
      <div class="login-card-form">
        <p>
          Si comme moi, vous n'aimez pas les formulaires de contact, vous pouvez
          simplement
          <b>copier mon adresse en cliquant sur le bouton ci-dessous&nbsp;:</b>
        </p>
        <button
          class="btn"
          v-clipboard="'f.chambinaud@gmail.com'"
          @click="ToggleCopied"
        >
          f.chambinaud@gmail.com
        </button>
        <p :class="{ copy: !isCopied, copied: isCopied }">
          Vous avez bien copié mon adresse mail !
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* .totalite {
  padding-top: 4rem;
} */
.titre {
  /* background-color: #219db2; */
  background-color: #397a89;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 0.7rem;
  margin-bottom: 2rem;
  position: relative;
  margin: 0 3rem;
}
h3 {
  font-family: "Montserrat", sans-serif;
  font-size: 1.2rem;
  font-weight: 500;
  /* margin-bottom: 0.4rem; */
  background-color: rgb(255, 255, 255);
  padding: 0rem 0.7rem;
  position: absolute;
}
.login-card-container {
  min-height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
  padding: 7rem 1.5rem;
  /* background: linear-gradient(to top, white, #5bb6c6); */
  /* background-color: rgba(24, 151, 168, 0.15); */
  background-color: rgba(57, 122, 137, 0.15);

  margin-top: 3rem;
}
.login-card-form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1.5rem;
  width: 100%;
  margin-top: 3rem;
}
.login-card-form-2 {
  display: flex;
  flex-direction: row;
  width: 100%;
  gap: 1.5rem;
}
.login-card-form .form-item {
  position: relative;
}
.login-card-form .form-item .form-item-icon {
  position: absolute;
  top: 0.82rem;
  left: 1.4rem;
  font-size: 1.3rem;
  opacity: 0.4;
}
input[type="text"] {
  border: none;
  outline: none;
  background: rgba(255, 255, 255, 0.7);
  padding: 1rem 1.5rem;
  padding-left: calc(1rem * 3.2);
  border-radius: 100px;
  width: 100%;
  transition: background 0.5s;
}
input[type="email"] {
  border: none;
  outline: none;
  background: rgba(255, 255, 255, 0.7);
  padding: 1rem 1.5rem;
  padding-left: calc(1rem * 3.2);
  border-radius: 100px;
  width: 100%;
  transition: background 0.5s;
}
.form-item {
  width: 100%;
}

input:focus {
  background: white;
}

#message {
  border-radius: 20px;
  width: 100%;
  height: 10rem;
  border: none;
  outline: none;
  padding: 1rem 1.5rem;
  background: rgba(255, 255, 255, 0.7);
  transition: background 0.5s;
}
#message:focus {
  background: white;
}
textarea {
  font-family: "Open sans";
  font-size: 0.9rem;
}
/* button {
  padding: 0.7rem 1.1rem;
  border-radius: 2rem;
  cursor: pointer;
  font-size: 1.1rem;
  border: none;
  box-shadow: inset 0px 0px 10px 3px #26a8bf;
  background: linear-gradient(to bottom, #5bb6c6 5%, #1897a8 100%);
  background-color: #5bb6c6;
  text-shadow: 0px 1px 1px #337985;
  color: white;
  font-weight: 600;
  font-family: "Montserrat", sans-serif;
}
button:hover {
  background: linear-gradient(to bottom, #5bb6c6 25%, #1897a8 100%);
  background-color: #5bb6c6;
  position: relative;
  top: -1px;
} */
button,
button::after {
  -webkit-transition: all 0.3s;
  -moz-transition: all 0.3s;
  -o-transition: all 0.3s;
  transition: all 0.3s;
}

button {
  padding: 0.7rem 1.1rem;
  /* border-radius: 0.5rem; */
  border-radius: 2rem;
  cursor: pointer;
  font-size: 1.1rem;
  /* border: 2px #219db2 solid; */
  border: 2px #397a89 solid;
  /* box-shadow: inset 0px 0px 10px 3px #26a8bf; */
  /* background: linear-gradient(to bottom, #5bb6c6 5%, #1897a8 100%); */
  background: none;
  /* text-shadow: 0px 1px 1px #337985; */
  font-weight: 600;
  font-family: "Montserrat", sans-serif;
  position: relative;
  /* color: #219db2; */
  color: #397a89;
  overflow: hidden;
}
button::before,
button::after {
  border: #fff 2px solid;
  border-radius: 2rem;
  /* background-color: #219db2; */
  background-color: #397a89;
  content: "";
  position: absolute;
  z-index: -1;
}
button:hover {
  color: #fff;
}
button:hover a {
  color: #fff;
}
.btn::before {
  height: 100%;
  left: 0;
  top: 0;
  width: 0;
}
.btn::after {
  height: 100%;
  left: 0;
  top: 0;
  width: 0;
}
.btn:hover::after {
  width: 100%;
}
p {
  font-size: 0.9rem;
  text-align: justify;
}
.copy {
  font-size: 0.8rem;
  font-weight: 600;
  color: #219db2;
}
.copied {
  /* display: none; */
  /* height: 0.8rem; */
  font-size: 0.8rem;
  font-weight: 600;
  color: rgba(33, 157, 178, 0);
}
#contact:target {
  padding-top: 6rem;
  margin-top: -6rem;
}
@media (min-width: 471px) {
  #contact:target {
    padding-top: 8.5rem;
    margin-top: -8.5rem;
  }
}
@media (min-width: 768px) {
  .titre {
    margin: 0 6rem;
  }
  .login-card-form {
    max-width: 50rem;
  }
}
@media (min-width: 1135px) {
  #contact:target {
    padding-top: 7rem;
    margin-top: -7rem;
  }
}
</style>