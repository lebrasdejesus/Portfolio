<script setup>
import ProjectsItem from "./ProjectsItem.vue";
import ImgLakson from "./icons/ImgLakson.vue";
import ImgProjet2 from "./icons/ImgProjet2.vue";
import ImgSuzuki from "./icons/ImgSuzuki.vue";
</script>


<template>
  <div id="reals">
    <div class="titre">
      <h3>RÉALISATIONS</h3>
    </div>
    <div class="grid-projects">
      <ProjectsItem>
        <template #image>
          <ImgLakson />
        </template>
        <template #texte
          ><a
            href="https://14h02m10s.github.io/ExerciceCopieSiteResto/#/"
            target="blank"
            >Reproduction d'un site vitrine</a
          ></template
        >
        Ceci est le projet le plus abouti que j'ai réalisé (en dehors de ce
        portfolio). Je l'ai commencé à la fin de mon stage (juin 2023) et l'ai
        continué chez moi. Le but ici n'est pas de créer, mais vraiment
        d'essayer de recopier un site vitrine, j'ai choisi celui du restaurant
        du
        <a href="https://lakson.fr/">Lakson</a> car il me semblait qu'il y avait
        plusieurs choses intéressantes à essayer de reproduire. <br />
        Il doit encore être amélioré car certaines choses étaient trop complexes
        lorsque j'ai commencé. Je n'ai donc pas fait les animations, ni le
        responsive, il n'est donc pour l'instant adapté que pour les écrans de
        plus de 1300 px de large.
      </ProjectsItem>

      <ProjectsItem>
        <template #image>
          <ImgProjet2 />
        </template>
        <template #texte
          ><a href="https://14h02m10s.github.io/TestVue-14h/" target="blank"
            >Divers exercices Html Css Javascript</a
          ></template
        >
        J'ai pris l'initiative de refaire un peu de js mais dans Vue.js, j'ai
        commencé par refaire de petits exercices faits en cours (pendant ma
        formation chez M2i). Puis, j'ai étoffé ce projet avec d'autres petites
        choses (color picker, ajout d'une image par l'utilisateur, copie d'une
        galerie photo sur dribbble), demandées par mon maître de stage. En
        parallèle j'ai construit une présentation avec une navbar, des titres,
        un texte de présentation. J'ai travaillé ce projet uniquement en desk,
        il est donc optimisé pour les écrans de minimum 1200 px.
      </ProjectsItem>

      <ProjectsItem>
        <template #image>
          <ImgSuzuki />
        </template>
        <template #texte
          ><a
            href="https://14h02m10s.github.io/ExerciceNavbarEtCarrouselSuzuki/"
            target="blank"
            >Reproduction de la navbar et slider du site Suzuki</a
          ></template
        >
        Voici le tout premier projet que j'ai fait avec Vue.js, en juin 2023,
        lors de mon stage. Mon maître de stage m'avait demandé de recopier le
        menu et le slider du
        <a href="https://concession.suzuki.fr/la-rochelle"
          >site suzuki concession</a
        >. <br />
        Rien n'est cliquable, c'est normal... et ce n'est pas optimisé pour le
        responsive, il est visible pour des écrans d'une taille maximale de 960
        px au maximum.
      </ProjectsItem>
    </div>
  </div>
</template>

<style scoped>
#reals {
  padding-top: 3rem;
  min-height: 100vh;
}
#reals:target {
  padding-top: 5rem;
  margin-top: -5rem;
}
.grid-projects {
  display: grid;
  grid-template-columns: 1fr;
}
.titre {
  background-color: #219db2;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 0.7rem;
  position: relative;
  /* margin: 0 3rem; */
  margin: 0.6rem 3rem 2rem 3rem;
}
h3 {
  font-family: "Montserrat", sans-serif;
  font-size: 1.2rem;
  font-weight: 500;
  background-color: rgb(255, 255, 255);
  padding: 0rem 0.7rem;
  position: absolute;
}
@media (min-width: 471px) {
  #reals:target {
    padding-top: 8rem;
    margin-top: -8rem;
  }
}
@media (min-width: 768px) {
  .titre {
    margin: 3rem 6rem 2rem 6rem;
  }
  #reals:target {
    padding-top: 5rem;
    margin-top: -5rem;
  }
}
@media (min-width: 1135px) {
  #reals:target {
    padding-top: 4rem;
    margin-top: -4rem;
  }
  .grid-projects {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    padding: 0 3rem;
  }
}
</style>