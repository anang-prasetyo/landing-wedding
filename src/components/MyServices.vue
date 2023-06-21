<template>
  <div class="container">
    <div class="label-1">MY SERVICES</div>
    <div class="c-title">
      <div class="strip"></div>
      <h2>All you need is on me</h2>
    </div>
    <div class="c-desc text-desc">I will take care of everything for you from event planing and curation to design and production.</div>
    <div class="images">
      <div class="s2-img1"></div>
      <div class="s2-img1"></div>
      <div class="s2-img1"></div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.container{
  padding: 0 5vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  gap: 1rem;
  & .c{
    &-title {
      position: relative;
      display: flex;
      justify-content: center;
      align-content: center;
      width: 100%;
      
      & .strip{
        height: 1px;
        width: 100%;
        background: var(--color4);
        position: absolute;
        top: 50%;
      }
      & h2{
        background: var(--color1);
        padding: 0 2rem;
      }
    }
    &-desc{
      max-width: calc(100vw/2);
    }
  }
}
.images{
  margin-top: 3rem;
  display: flex;
  flex-direction: column;
  gap: .5rem;
  width: 100%;
  & .s2-img1{
    background: var(--color6);
    height: 24rem;
  }
}
@media (min-width: 1024px) {
  .images{
    margin-top: 1rem;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    & .s2-img1{
      height: 24rem;
      width: calc((100% / 3) - .5rem);
    }
  }
  .container{
    padding: 0 7vw;
    & .c{
      &-desc{
        max-width: calc(100vw/3);
      }
    }
  }
}
</style>