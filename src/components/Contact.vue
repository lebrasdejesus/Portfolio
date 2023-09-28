<template>
  <div class="totalite" id="contact">
    <div class="titre">
      <h3>CONTACT</h3>
    </div>
    <div class="login-card-container">
      <div class="login-card">
        <!-- <div class="login-card-logo">
          <img src="../assets/logo.png" alt="logo" />
        </div> -->
        <!-- <div class="login-card-header">
          <div>Veuillez remplir le formulaire ci-dessous</div>
        </div> -->
        <form class="login-card-form">
          <div class="login-card-form-2">
            <div class="form-item">
              <span class="form-item-icon material-symbols-rounded"
                >person</span
              >
              <input type="text" placeholder="Nom" id="nom" required />
            </div>
            <div class="form-item">
              <span class="form-item-icon material-symbols-rounded"
                >person</span
              >
              <input type="text" placeholder="Prénom" id="prenom" required />
            </div>
          </div>

          <div class="form-item">
            <span class="form-item-icon material-symbols-rounded">mail</span>
            <input type="email" placeholder="Email" id="email" required />
          </div>
          <div class="form-item">
            <textarea id="message" name="message" required></textarea>
          </div>
          <button type="submit">Envoyer</button>
        </form>
      </div>
    </div>
  </div>
</template>

<style scoped>
.totalite {
  min-height: 100vh;
}
.titre {
  background-color: #219db2;
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
  /* min-height: 100vh; */
  /* background: #337985; */
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  /* width: 100%; */
  padding: 3rem;
  background: linear-gradient(to top, white, #5bb6c6);
  margin: 3rem;
}
/* Login Card */
.login-card {
  /* width: 75%; */
  /* background: rgba(255, 255, 255, 0.5); */
  /* padding: 4rem; */
  /* border-radius: 10px; */
  position: relative;
}

/* Login Card Logo */
/* .login-card-logo {
  margin-bottom: 2rem;
} */

/* .login-card-logo img {
  width: 60px;
} */

/* Login Card Standard */
/* .login-card-logo,
.login-card-header {
  text-align: center;
} */

/* Login Card Header */
/* .login-card-header {
  margin-bottom: 2rem;
} */

/* .login-card-header div {
  font-size: calc(1rem * 0.8);
  opacity: 0.8;
} */

/* Login Card Form */
.login-card-form {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}
.login-card-form-2 {
  display: flex;
  flex-direction: row;
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

/* .login-card-form .form-item-other {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-size: calc(1rem * 0.8);
  margin-bottom: 0.5rem;
} */

/* Login Card Form Elements */
.login-card input[type="text"] {
  border: none;
  outline: none;
  background: rgba(255, 255, 255, 0.3);
  padding: 1rem 1.5rem;
  padding-left: calc(1rem * 3.5);
  border-radius: 100px;
  width: 100%;
  transition: background 0.5s;
}
.login-card input[type="email"] {
  border: none;
  outline: none;
  background: rgba(255, 255, 255, 0.3);
  padding: 1rem 1.5rem;
  padding-left: calc(1rem * 3.5);
  border-radius: 100px;
  width: 100%;
  transition: background 0.5s;
}
.form-item {
  width: 100%;
}

.login-card input:focus {
  background: white;
}

#message {
  border-radius: 20px;
  width: 100%;
  height: 10rem;
  border: none;
  outline: none;
  padding: 1rem 1.5rem;
  background: rgba(255, 255, 255, 0.3);
  transition: background 0.5s;
}
#message:focus {
  background: white;
}
textarea {
  font-family: "Open sans";
  font-size: 0.9rem;
}

button {
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
  /* width: 50%; */
}

button:hover {
  background: linear-gradient(to bottom, #5bb6c6 25%, #1897a8 100%);
  background-color: #5bb6c6;
  position: relative;
  top: -1px;
}
@media (min-width: 768px) {
  .totalite {
    padding: 3rem 6rem;
    width: 100%;
  }
  /* .login-card-container {
    padding: 2rem 0;
  }

  .login-card {
    width: 280px;
    padding: 2rem;
  } */
}
</style>