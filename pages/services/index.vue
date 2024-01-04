<script setup lang="ts">
import data from '../../composables/rpData';

const serviceList = data.services;
</script>

<template>
  <section id="services" class="main__contain">
    <div class="services__contain">
    <h2>Our services</h2>
    <div class="links" v-for="(service, idx) in serviceList" :key="idx">
      <nuxt-link :to="service.serviceSlug">
        {{ service.title }}
      </nuxt-link>
    </div>
  </div>
  </section>
</template>

<style lang="scss" scoped>
#services {
  .services__contain {
    width: 100%;
    max-width: var(--max-width);
  }
}
</style>