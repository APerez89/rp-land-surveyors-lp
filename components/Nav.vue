<script setup lang="ts">
</script>

<template>
  <nav id="nav" class="main__contain">
    <div class="nav__wrap">
      <div class="logo__wrap">
        <nuxt-link to="/">
          <img src="main-logo-small.webp" alt="">
        </nuxt-link>
      </div>
      <div class="nav__items">
        <div class="item">
          <nuxt-link to="about">About</nuxt-link>

        </div>
        <div class="item">
          <nuxt-link to="services">Services</nuxt-link>

        </div>
        <div class="item">
          <nuxt-link to="projects">Projects</nuxt-link>

        </div>
        <div class="item">
          <nuxt-link to="contact">Contact</nuxt-link>

        </div>
      </div>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
#nav {
  .nav__wrap {
    width: 100%;
    display: flex;
    max-width: var(--max-width);
    justify-content: space-between;

    .nav__items {
      display: inline-flex;
      align-items: flex-end;

      .item {
        display: contents;

        a {
          padding: 10px 25px;
          text-decoration: none;
        }
      }
    }
  }
}
</style>