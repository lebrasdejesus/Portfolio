<template>
  <div class="item">
    <div class="img">
      <slot name="image"></slot>
    </div>

    <div class="details">
      <h3>
        <slot name="texte"></slot>
      </h3>
      <slot></slot>
    </div>
  </div>
</template>
  
  <style scoped>
.item {
  display: grid;
  grid-template-columns: 1fr;
  /* grid-gap: 0.2rem; */
  /* border: 1px rgba(208, 208, 208, 0.3) solid; */
  margin-top: 1rem;
  padding: 1rem 3rem;
}
.img {
  width: 100%;
  height: fit-content;
  /* border: 1px purple dashed; */
  display: block;
}
.details {
  flex: 1;
  margin: 0 1rem 1rem 1rem;
}
h3 {
  font-family: "Montserrat", sans-serif;
  font-size: 1.2rem;
  font-weight: 700;
  margin-bottom: 0.4rem;
  /* border: 1px black solid; */
}

@media (min-width: 768px) {
  .item {
    /* margin-top: 0;
    padding: 0.4rem 0 1rem calc(var(--section-gap) / 2); */
    display: grid;
    /* grid-template-columns: repeat(2, 1fr); */
    grid-template-columns: 1fr 2fr;
    grid-gap: 0.2rem;
    /* border: 1px rgba(208, 208, 208, 0.3) solid; */
    padding: 1rem 6rem;
  }
}
</style>