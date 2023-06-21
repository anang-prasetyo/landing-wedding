<template>
  <div class="container">
    <div class="c-aboutus">
      <div class="c-left">
        <div>
          <div class="label-1">ABOUT US</div>
        </div>
        <h2>Interior design that matters.</h2>
        <div class="c-left-bot">
          <div class="c-left-bot-left">
            <div class="c-left-bot-left-top">1K+</div>
            <div class="c-left-bot-left-bot text-desc">Regular ... in every month</div>
          </div>
          <div class="c-left-bot-right">
            <div class="c-left-bot-right-top">5+</div>
            <div class="c-left-bot-right-bot text-desc">Years of experience</div>
          </div>
        </div>
      </div>
      <div class="c-right">
        <div class="c-right-left"></div>
        <div class="c-right-right"></div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container{
  padding: 0 5vw;
}
.c{
  &-right{
    display: flex;
    gap: .5rem;
    width: 100%;
    height: 25rem;
    &-left, &-right{
      display: flex;
      background: var(--color6);
      height: 20rem;
      width: calc((100% / 2) - .5rem);
    }
    &-left{
      align-self: flex-start;
    }
    &-left{
      align-self: flex-end;
    }
  }
  &-left{
    display: flex;
    flex-direction: column;
    gap: 2rem;
    justify-content: center;
    &-bot{
      display: flex;
      gap: 1rem;
      &-left, &-right{
        &-top{
          font-size: 1.25rem;
          font-weight: 700;
        }
        &-bot{
          font-size: .8rem;
        }
      }
    }
  }
  &-aboutus{
    width: 100%;
    padding: 2rem;
    border: 1px solid var(--color4);
    display: flex;
    flex-direction: column;
    gap: 4rem;
  }
}
@media (min-width: 1024px) {
  .container{
    padding: 0 7vw;
  }
  .c{
    &-aboutus{
      flex-direction: row;
      padding: 2rem 7rem;
      gap: 7rem;
    }
    &-left{
      max-width: 30vw;
    }
  }
}
</style>