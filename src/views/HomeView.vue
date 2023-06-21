<script setup>
import AboutUs from "../components/AboutUs.vue";
import HelloWorld from "../components/HelloWorld.vue";
import MyServices from "../components/MyServices.vue";
import OnInstagram from "../components/OnInstagram.vue";
import OrderNow from "../components/OrderNow.vue";

</script>

<template>
  <main>
    <section>
      <hello-world />
    </section>
    <section>
      <my-services />
    </section>
    <section>
      <about-us />
    </section>
    <section>
      <on-instagram />
    </section>
    <section>
      <order-now />
    </section>
    <section>
      <div class="container">
        <div class="order-now">
          <div class="order-now-top">
            <div class="order-now-top-left">
              <div class="order-now-top-left-title">
                <h3>Contact us</h3>
              </div>
              <div class="order-now-top-left-desc">
                <div>Surakarta, Indonesia</div>
                <div>+62 821 3393 8464</div>
              </div>
            </div>
            <div class="order-now-top-right">
              <div class="order-now-top-right-title">
                <h3>Working hours</h3>
              </div>
              <div class="order-now-top-right-desc">
                <div>Monday-Friday : 08.00 - 06.00</div>
                <div>Saturday-Sunday : 08.00 - 06.00</div>
              </div>
            </div>
          </div>
          <div class="order-now-bot">
            <div class="sosmed">
              <div></div>
              <div></div>
              <div></div>
            </div>
            <div class="cr">Copyright 2023 Anang Prasetyo</div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<style lang="scss" scoped>
main{
  // padding: 0 5vw;
  padding-bottom: 3rem;
  display: flex;
  flex-direction: column;
  gap: 7rem;
}
.container{
  display: flex;
  flex-direction: columns;
  align-items: center;
  gap: 1rem;
}
.order-now{
  padding: 0 5vw;
  flex-direction: column;
  gap: 3rem;
  &, &-top, &-bot{
    width: 100%;
    display: flex;
  }
  &-top{
    gap: 2rem;
    &-left, &-right{
      display: flex;
      flex-direction: column;
      align-items: center;
      width: calc(100vw / 2);
      border: 1px solid var(--color4);
      padding: 3rem 0;
      gap: 1rem;
      &-desc{
        color: var(--color-border);
      }
    }
  }
  &-bot{
    flex-direction: column;
    align-items: center;
    gap: 2rem;
    & .sosmed{
      display: flex;
      gap: 1rem;
      & div{
        height: 2rem;
        width: 2rem;
        background: var(--color6);
        border-radius: 5px;
      }
    }
    & .cr{
      color: var(--color-border);
    }
  }
}


@media (min-width: 1024px) {
  // main{
  //   padding: 0 7vw;
  // }
  .order-now{
        padding: 0 7vw;
    }
}
</style>