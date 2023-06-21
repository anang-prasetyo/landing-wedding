<template>
  <nav>
    <div>
      <RouterLink to="/">Home</RouterLink>
      <a>Explore</a>
      <RouterLink to="/about">About</RouterLink>
      <a>Contact</a>
      <a>Price</a>
    </div>
    <div>
      <button>Let's talk</button>
    </div>
  </nav>
</template>

<script setup>
import { RouterLink } from 'vue-router'
</script>

<style lang="scss" scoped>
nav{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 5vw;
  gap: 2rem;
  & div{
    display: flex;
    gap: 2rem;
    & a{
      text-decoration: none;
      color: currentColor;
      cursor: pointer;
    }
  }
}
button{
  background: var(--color1);
  padding: .75rem 1.5rem;
  color: var(--color3);
  border: 2px solid var(--color4);
  border-radius: 5px;
  font-weight: 600;
  transition: all .25s ease;
  &:hover{
    border: 2px solid var(--color3);
  }
}
@media (min-width: 1024px) {
  nav{
    padding: 1rem 7vw;
  }
}
</style>