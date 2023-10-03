<script setup>
import PresentationItem from "./PresentationItem.vue";
import PresentationItemSkills from "./PresentationItemSkills.vue";
</script>

<template>
  <div class="espace-nav">
    <div id="head">
      <PresentationItem>
        <template #heading>PRÉSENTATION</template>
        <div class="photo-et-texte">
          <div class="photo">
            <img
              src="../assets/IMG20230829161457(3)(1)(2).jpg"
              alt="photo profil"
            />
          </div>
          <div>
            <p>
              Bonjour,<br /><br />je suis ravie de vous accueillir sur mon
              portfolio où mon expérience professionnelle se marie avec ma
              passion naissante pour le développement.
              <b>J'ai en effet travaillé 20 ans, en tant que maquettiste</b>,
              dans diverses entreprises où j'ai perfectionné mon sens du détail,
              ma capacité à faire des délivrables à la fois communiquants,
              harmonieux et respectueux des différentes chartes graphiques.
              <br /><br />Depuis début 2023, j'entame ma reconversion dans
              l'univers du développement. J'ai suivi la
              <b>formation "Développeur .Net fullstack"</b> chez M2i pendant 4
              mois (à temps complet) suivie d'un mois de stage. Je suis encore
              débutante, mais j'ai à cœur de progresser et
              <b>j'apprends tous les jours un peu plus</b>. Mon portfolio est
              justement là pour vous montrer mes réalisations dans ce nouveau
              domaine, où le graphisme rencontre le code. <br /><br />J'ai
              décidé de continuer mon apprentissage avec la <b>3W Academy</b>,
              au rythme de 3 semaines en entreprise et une semaine en cours,
              <b
                >je recherche donc une entreprise pour un contrat en alternance
                en tant qu'intégrateur/developpeur front-end</b
              >
              donc n'hésitez pas à me
              <span
                ><a href="#contact"><b>contacter</b></a></span
              >
              si vous pensez que mon profil peut vous intéresser.
            </p>
          </div>
        </div>
        <div class="container-button">
          <button>
            <a
              href="../../src/assets/CV-F-CHAMBINAUD-220923_compressed.pdf"
              target="blank"
              >Télécharger mon cv</a
            >
          </button>
        </div>
      </PresentationItem>

      <div class="super-container-hardSkills">
        <div class="container-hardSkills-titre">
          <div class="titre-skills"><h3>Compétences techniques</h3></div>
          <div class="container-two-containers-hard-skills">
            <div class="two-containers-hard-skills margin-bottom">
              <div class="container-hardSkills">
                <PresentationItemSkills>
                  <template #image>
                    <img src="../assets/pictos/HTML5.svg" alt="picto Html" />
                  </template>
                  <template #texte><p>HTML 5</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/CSS3_logo.svg"
                      alt="picto Css"
                      class="height100"
                    />
                  </template>
                  <template #texte><p>CSS 3</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Unofficial_JavaScript_logo_2.svg"
                      alt="picto Js"
                    />
                  </template>
                  <template #texte><p>JavaScript</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Vuejs_Logo_2.svg"
                      alt="picto Vue"
                    />
                  </template>
                  <template #texte><p>Vue.js</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/React_Logo.svg"
                      alt="picto React"
                    />
                  </template>
                  <template #texte><p>React</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Tailwind_CSS_Logo.svg"
                      alt="picto Tailwind"
                    />
                  </template>
                  <template #texte><p>Tailwind</p></template>
                </PresentationItemSkills>
              </div>
              <div class="container-hardSkills">
                <PresentationItemSkills>
                  <template #image>
                    <img src="../assets/pictos/Figma.svg" alt="picto Figma" />
                  </template>
                  <template #texte><p>Figma</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Adobe_XD_CC_icon.svg"
                      alt="picto XD"
                    />
                  </template>
                  <template #texte><p>Adobe Xd</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Adobe_InDesign_CC_logo.svg"
                      alt="picto Indesign"
                    />
                  </template>
                  <template #texte><p>Adobe Indesign</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Adobe_Photoshop_CC_icon.svg"
                      alt="picto Photoshop"
                    />
                  </template>
                  <template #texte><p>Adobe Photoshop</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Adobe_Illustrator_CC_icon.svg"
                      alt="picto Illustrator"
                    />
                  </template>
                  <template #texte><p>Adobe Illustrator</p></template>
                </PresentationItemSkills>
                <PresentationItemSkills>
                  <template #image>
                    <img
                      src="../assets/pictos/Photopea_logo.svg"
                      alt="picto Photopea"
                    />
                  </template>
                  <template #texte><p>Photopea</p></template>
                </PresentationItemSkills>
              </div>
            </div>
          </div>
        </div>
        <div class="container-hardSkills-titre">
          <div class="titre-skills"><h3>Savoir-être</h3></div>
          <div class="container-hardSkills">
            <ul>
              <li>Réactive</li>
              <li>Rigoureuse</li>
              <li>Créative</li>
              <li>Perséverante</li>
              <li>À l'écoute</li>
              <li>Sens de l'organisation</li>
              <li>Maîtrise avancée du français</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.espace-nav {
  /* margin-top: 11.5rem; */
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  padding-top: 3rem;
}
.super-container-hardSkills {
  display: flex;
  flex-direction: column;
  background-color: rgba(24, 151, 168, 0.15);
  margin-bottom: 2rem;
  padding: 2rem 0;
}
.container-hardSkills-titre {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0 auto;
}
.titre-skills {
  display: flex;
  justify-content: center;
  line-height: 0.7rem;
  margin-bottom: 0.6rem;
  /* color: white; */
}
.container-two-containers-hard-skills {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.two-containers-hard-skills {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: left;
}
.margin-bottom {
  padding-bottom: 2rem;
}
.container-hardSkills {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: left;
  width: fit-content;
}
.container-button {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 1.5rem 0;
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
  /* margin-bottom: 1rem; */
}

a:hover {
  text-decoration: none;
}
button:hover {
  /* background: linear-gradient(to bottom, #1897a8 5%, #5bb6c6 100%);
  background-color: #1897a8; */
  background: linear-gradient(to bottom, #5bb6c6 25%, #1897a8 100%);
  background-color: #5bb6c6;
  position: relative;
  top: -1px;
}
/* button:active {
  position: relative;
  top: 1px;
} */
p {
  font-size: 0.9rem;
  text-align: justify;
}
span {
  background-color: #219db2;
}
a {
  color: white;
}
/* #head:target {
  padding-top: 14.4rem;
  margin-top: -14.4rem;
} */
#head:target {
  padding-top: 7rem;
  margin-top: -7rem;
}
.photo-et-texte {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.photo {
  border-radius: 10rem;
  width: 7rem;
  height: 7rem;
}
.photo img {
  width: 7rem;
  border-radius: 10rem;
  border: 2px #219db2 solid;
}
.height100 {
  height: 100%;
}
h3 {
  margin-bottom: 1rem;
  text-align: center;
  font-size: 1.1rem;
}
/* .container-hardSkills p {
  color: white;
} */
li {
  font-weight: 600;
  padding: 0.2rem;
  /* color: white; */
}
@media (min-width: 471px) {
  .espace-nav {
    padding-top: 6rem;
  }
  #head:target {
    padding-top: 8rem;
    margin-top: -8rem;
  }
}
@media (min-width: 768px) {
  .espace-nav {
    padding-top: 5.5rem;
  }
  #head:target {
    padding-top: 5.5rem;
    margin-top: -5.5rem;
  }

  .photo-et-texte {
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: start;
  }
  .photo {
    width: 8.5rem;
    height: 8.5rem;
    margin-right: 2rem;
  }
  .photo img {
    width: 8.5rem;
    border: 2px #219db2 solid;
  }
  .super-container-hardSkills {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: start;
  }
  .container-two-containers-hard-skills {
    display: flex;
    flex-direction: row;
  }
  .two-containers-hard-skills {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: left;
  }
  .container-hardSkills-titre {
    display: flex;
    flex-direction: column;
    justify-content: left;
    margin: 2rem;
  }
  .container-hardSkills {
    margin: 0 2rem;
  }
  .margin-bottom {
    padding-bottom: 0rem;
  }
}
@media (min-width: 1135px) {
  #head:target {
    padding-top: 4rem;
    margin-top: -4rem;
  }

  .photo-et-texte {
    display: flex;
    flex-direction: row;
    justify-content: left;
    align-items: start;
  }
  .photo {
    width: 10rem;
    height: 10rem;
    margin-right: 3rem;
  }
  .photo img {
    width: 10rem;
    border: 2px #219db2 solid;
  }
  p {
    font-size: 1rem;
  }
  .container-hardSkills-titre {
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: left;
    margin: 2rem;
  }
  .container-hardSkills {
    display: flex;
    flex-direction: column;
  }
}
</style>