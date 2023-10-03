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

    <ProjectsItem>
      <template #image>
        <ImgLakson />
      </template>
      <template #texte
        ><a
          href="https://14h02m10s.github.io/ExerciceCopieSiteResto/#/"
          target="blank"
          >Reproduction du site d'un restaurant</a
        ></template
      >
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc id elit
      tempor, bibendum sem sed, condimentum lorem. Vivamus nec iaculis augue.
      Donec eget auctor mi. Cras quis elit nec purus placerat efficitur sed nec
      tortor. Phasellus sagittis interdum tempus. Phasellus eu ligula nec mi
      posuere suscipit. Phasellus tincidunt elit ante, in mollis diam fringilla
      blandit. Nam pulvinar metus magna, sed ornare metus pellentesque lacinia.
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
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc id elit
      tempor, bibendum sem sed, condimentum lorem. Vivamus nec iaculis augue.
      Donec eget auctor mi. Cras quis elit nec purus placerat efficitur sed nec
      tortor. Phasellus sagittis interdum tempus. Phasellus eu ligula nec mi
      posuere suscipit. Phasellus tincidunt elit ante, in mollis diam fringilla
      blandit. Nam pulvinar metus magna, sed ornare metus pellentesque lacinia.
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
      https://concession.suzuki.fr/la-rochelle <br />
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc id elit
      tempor, bibendum sem sed, condimentum lorem. Vivamus nec iaculis augue.
      Donec eget auctor mi. Cras quis elit nec purus placerat efficitur sed nec
      tortor. Phasellus sagittis interdum tempus. Phasellus eu ligula nec mi
      posuere suscipit. Phasellus tincidunt elit ante, in mollis diam fringilla
      blandit. Nam pulvinar metus magna, sed ornare metus pellentesque lacinia.
    </ProjectsItem>
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
.titre {
  background-color: #219db2;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 0.7rem;
  /* margin-bottom: 2rem; */
  position: relative;
  /* margin: 0 3rem; */
  margin: 0.6rem 3rem 2rem 3rem;
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
@media (min-width: 471px) {
  #reals:target {
    padding-top: 8rem;
    margin-top: -8rem;
  }
}
@media (min-width: 768px) {
  .titre {
    margin: 3rem 3rem 2rem 3rem;
  }
  #reals:target {
    padding-top: 5rem;
    margin-top: -5rem;
  }
}
@media (min-width: 1146px) {
  #reals:target {
    padding-top: 4rem;
    margin-top: -4rem;
  }
}
</style>