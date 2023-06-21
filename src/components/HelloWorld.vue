<template>
  <div class="hello-world">
    <main>
      <section>
        <h1>Hi There This is — Anang Prasetyo</h1>
        <div class="s1-desc text-desc">Floral Designer, Wedding Planner, and Event Enthusiast who creates memorable moments for special occasions.</div>
        <button class="btn-1">Get in touch</button>
      </section>
      <section>
        <div class="s2">
          <div class="s2-img1"></div>
          <div class="s2-img2"></div>
          <div class="s2-img3"></div>
        </div>
      </section>
    </main>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
.hello-world {
  & main{
    padding: 1rem 5vw;
    margin-top: 3rem;
    display: flex;
    flex-direction: column;
    gap: 5rem;
    & section {
      & .s1-desc{
        margin: 2rem 0;
      }
      & .s2{
        position: relative;
        height: 26rem;
        &-img{
          &1, &2, &3{
            position: absolute;
          }
          &1{
            background: var(--color6);
            top: 0;
            left: 50%;
            transform: translate(-50%, 0%);
            width: 22rem;
            height: 26rem;
            z-index: 2;
          }
          &2{
            background: var(--color5);
            top: 10rem;
            left: 0;
            width: 9rem;
            height: 12rem;
            z-index: 3;
            border-top-left-radius: 6rem;
            border-top-right-radius: 6rem;
          }
          &3{
            background: var(--color5);
            top: 4rem;
            right: 0;
            width: 9rem;
            height: 12rem;
            z-index: 1;
          }
        }
      }
    }
  }
}

@media (min-width: 1024px) {
  .hello-world {
    & main{
      padding: 0 7vw;
      flex-direction: row;
      justify-content: space-between;
      gap: 3rem;
      & section{
        max-width: 40vw;
        min-width: 40vw;
        & h1{
          max-width: 25vw;
        }
        & .s2{
          height: auto;
        }
      }
    }
  }
}
</style>