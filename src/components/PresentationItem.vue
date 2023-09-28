<template>
  <div class="item">
    <div class="details">
      <div class="titre">
        <h3>
          <slot name="heading"></slot>
        </h3>
      </div>
      <div class="texteprez">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<style scoped>
.item {
  /* margin-top: 1rem; */
  display: flex;
  position: relative;
  padding: 3rem 3rem;
}
.details {
  /* flex: 1; */
}
.titre {
  background-color: #219db2;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 0.7rem;
  margin-bottom: 2rem;
  position: relative;
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
/* .texteprez {
  margin-bottom: 0.5rem;
} */
@media (min-width: 768px) {
  .item {
    padding: 3rem 6rem;
  }
}
@media (min-width: 1024px) {
  .item {
    /* margin-top: 0; */
    /* padding: 0.4rem 0 1rem calc(var(--section-gap) / 2); */
  }
}
</style>
