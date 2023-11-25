<script setup lang="ts">
defineProps<{
  message: string
  link: string
}>()
</script>

<template>
  <div id="button__contain" class="main__contain">
    <div class="button__wrapper">
      <nuxt-link :to="link">
        {{ message }}
      </nuxt-link>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#button__contain {
  margin-top: 25px;
  .button__wrapper {
    width: 100%;
    position: relative;
    
    a {
      position: absolute;
      font-family: 'Raleway', sans-serif;
      color: var(--light-white);
      font-size: 1.1rem;
      padding: 15px 40px;
      background-color: var(--rp-red);
      border-radius: 50px;
      box-shadow: 0px 3px 15px rgba(0,0,0,0.3);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 1.2px;
      transition: all 0.2s ease-in-out;

      &:hover {
        background-color: var(--rp-light-red);
        box-shadow: 0px 3px 15px rgba(0,0,0,0.5);
        transform: translateY(-5px);
      }
    }
  }
}
</style>