<template>
  <section id="project" class="main__contain">
    <div class="project__contain">
      <h2>
        Welcome to {{ projectInfo?.title }}
      </h2>
    </div>
  </section>
</template>

<script setup lang="ts">
import data from '../../composables/rpData';

const route = useRoute();
const { slug } = route.params;
const projectInfo = data.projects.find(i => i.slug === slug);

</script>

<style lang="scss" scoped>
#project {
  .project__contain {
    width: 100%;
    max-width: var(--max-width);
  }
} 
</style>