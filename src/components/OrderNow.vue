<template>
  <div class="lets-talk">
    <h2>Are you ready to plan a special day</h2>
    <div class="lets-talk-desc text-desc">We will take care of everything for you from event planning and curation to design and production</div>
    <button class="btn-1">Let's talk</button>
  </div>
</template>

<style lang="scss" scoped>
.lets-talk{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  gap: 1rem;
  background: var(--color4);
  width: 100%;
  padding: 4rem 2rem;
}

@media (min-width: 1024px) {
  .lets-talk{
    & h2, &-desc{
      max-width: 30vw;
    }
  }
}
</style>