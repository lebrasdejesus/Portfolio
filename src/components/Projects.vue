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

<!-- <template>
  <div class="container">
    <div class="one"></div>
    <div class="two"></div>
    <div class="three"></div>
  </div>
</template> -->
<style scoped>
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
#reals {
  min-height: 100vh;
}
#reals:target {
  padding-top: 14.4rem;
  margin-top: -14.4rem;
}

@media (min-width: 471px) {
  #reals:target {
    padding-top: 11rem;
    margin-top: -11rem;
  }
}
@media (min-width: 768px) {
  #reals:target {
    padding-top: 8.5rem;
    margin-top: -8.5rem;
  }
  .titre {
    margin: 0 6rem;
  }
}
@media (min-width: 1146px) {
  #reals:target {
    padding-top: 7rem;
    margin-top: -7rem;
  }
}
/* .container {
  display: grid;
  grid-template-columns: 1fr;
  grid-gap: 2rem;
  border: 1px black solid;
  margin-top: 2rem;
}
.one {
  background-color: aqua;
  height: 5rem;
}
.two {
  background-color: rgb(33, 92, 92);
  height: 5rem;
}
.three {
  background-color: rgb(255, 0, 208);
  height: 5rem;
}

@media (min-width: 768px) {
  .container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 2rem;
  }
} */
</style>