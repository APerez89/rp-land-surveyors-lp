<template>
  <section id="service" class="main__contain">
    <div class="service__contain">
      <h2>
        Welcome to {{ serviceInfo?.title }}
      </h2>
    </div>
  </section>
</template>

<script setup lang="ts">
import data from '../../composables/rpData';

const route = useRoute();
const { slug } = route.params;
const serviceInfo = data.services.find(i => i.slug === slug);

</script>

<style lang="scss" scoped>
#service {
  .service__contain {
    width: 100%;
    max-width: var(--max-width);
  }
} 
</style>