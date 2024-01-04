<template>
  <div>
    <h2>
      Welcome to {{ serviceInfo?.title }}
    </h2>
  </div>
</template>

<script setup lang="ts">
import data from '../../composables/rpData';

const route = useRoute();
const { slug } = route.params;
const serviceInfo = data.services.find(i => i.slug === slug);

// definePageMeta({
//   layout: 'default'
// })
</script>

<style lang="scss" scoped>
  
</style>