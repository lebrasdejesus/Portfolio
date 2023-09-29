<template>
  <div class="item">
    <div class="img">
      <slot name="image"></slot>
    </div>

    <div class="details">
      <p>
        <slot name="texte"></slot>
      </p>
    </div>
  </div>
</template>

<style scoped>
.item {
  display: flex;
  flex-direction: row;
  justify-content: left;
  align-items: center;
  padding: 0.3rem;
  width: fit-content;
}
.details {
  /* flex: 1; */
  font-weight: 600;
  font-size: 0.9rem;
}
.img {
  width: 3rem;
  height: 2.5rem;
  padding-right: 0.5rem;
  display: flex;
  justify-content: center;
}

@media (min-width: 768px) {
  .item {
    /* padding: 3rem 6rem; */
  }
}
@media (min-width: 1024px) {
  .item {
    /* margin-top: 0; */
    /* padding: 0.4rem 0 1rem calc(var(--section-gap) / 2); */
  }
}
</style>
