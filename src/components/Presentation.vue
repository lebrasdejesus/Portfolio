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
              domaine, où le graphisme rencontre le code. <br /><br />N'hésitez
              pas à me
              <span
                ><a href="#contact"><b>contacter</b></a></span
              >
              si vous voulez en savoir plus sur moi et, pourquoi pas, me
              proposer un
              <b
                >contrat en alternance en tant qu'intégrateur/developpeur
                front-end</b
              >
              puisque j'ai décidé de continuer mon apprentissage avec la
              <b>3W Academy</b>, au rythme de 3 semaines en entreprise et une
              semaine en cours.
            </p>
            <div class="container-button">
              <button>
                <a
                  href="../../src/assets/CV-F-CHAMBINAUD-220923_compressed.pdf"
                  target="blank"
                  >Télécharger mon cv</a
                >
              </button>
            </div>
          </div>
        </div>
      </PresentationItem>
      <PresentationItemSkills>
        <template #image>
          <img src="../assets/pictos/Adobe_XD_CC_icon.svg" alt="picto XD" />
        </template>
        <template #texte><p>Adobe Xd</p></template>
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
    </div>
    <!-- <PresentationItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Tooling</template>

    This project is served and bundled with
    <a
      href="https://vitejs.dev/guide/features.html"
      target="_blank"
      rel="noopener"
      >Vite</a
    >. The recommended IDE setup is
    <a href="https://code.visualstudio.com/" target="_blank" rel="noopener"
      >VSCode</a
    >
    +
    <a
      href="https://github.com/johnsoncodehk/volar"
      target="_blank"
      rel="noopener"
      >Volar</a
    >. If you need to test your components and web pages, check out
    <a href="https://www.cypress.io/" target="_blank" rel="noopener">Cypress</a>
    and
    <a href="https://on.cypress.io/component" target="_blank" rel="noopener"
      >Cypress Component Testing</a
    >.

    <br />

    More instructions are available in <code>README.md</code>.
  </PresentationItem>

  <PresentationItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Ecosystem</template>

    Get official tools and libraries for your project:
    <a href="https://pinia.vuejs.org/" target="_blank" rel="noopener">Pinia</a>,
    <a href="https://router.vuejs.org/" target="_blank" rel="noopener"
      >Vue Router</a
    >,
    <a href="https://test-utils.vuejs.org/" target="_blank" rel="noopener"
      >Vue Test Utils</a
    >, and
    <a href="https://github.com/vuejs/devtools" target="_blank" rel="noopener"
      >Vue Dev Tools</a
    >. If you need more resources, we suggest paying
    <a
      href="https://github.com/vuejs/awesome-vue"
      target="_blank"
      rel="noopener"
      >Awesome Vue</a
    >
    a visit.
  </PresentationItem>

  <PresentationItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Community</template>

    Got stuck? Ask your question on
    <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Vue Land</a
    >, our official Discord server, or
    <a
      href="https://stackoverflow.com/questions/tagged/vue.js"
      target="_blank"
      rel="noopener"
      >StackOverflow</a
    >. You should also subscribe to
    <a href="https://news.vuejs.org" target="_blank" rel="noopener"
      >our mailing list</a
    >
    and follow the official
    <a href="https://twitter.com/vuejs" target="_blank" rel="noopener"
      >@vuejs</a
    >
    twitter account for latest news in the Vue world.
  </PresentationItem>

  <PresentationItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Support Vue</template>

    As an independent project, Vue relies on community backing for its
    sustainability. You can help us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener"
      >becoming a sponsor</a
    >.
  </PresentationItem> -->
  </div>
</template>
<style scoped>
.espace-nav {
  margin-top: 11.5rem;
  /* position: relative; */
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.container-button {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 1.5rem;
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
#head:target {
  padding-top: 14.4rem;
  margin-top: -14.4rem;
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
@media (min-width: 471px) {
  .espace-nav {
    margin-top: 8rem;
    /* margin-top: 5rem; */
  }
  #head:target {
    padding-top: 8rem;
    margin-top: -8rem;
  }
  .container-button {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
@media (min-width: 768px) {
  .espace-nav {
    margin-top: 5.5rem;
  }
  #head:target {
    padding-top: 5.5rem;
    margin-top: -5.5rem;
  }
  .container-button {
    display: flex;
    justify-content: left;
    align-items: center;
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
}
@media (min-width: 1135px) {
  .espace-nav {
    margin-top: 4rem;
  }
  #head:target {
    padding-top: 4rem;
    margin-top: -4rem;
  }
  .container-button {
    display: flex;
    justify-content: left;
    align-items: center;
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
}
</style>