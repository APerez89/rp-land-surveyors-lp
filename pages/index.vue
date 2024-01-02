<template>
  <div id="index__contain" class="main__contain">
    <div class="main__wrap">
      <Welcome />
      <WhyRP />
      <Divider />
      <ProjectsCompleted />
      <HighlightProjects />
    </div>
  </div>
</template>

<script setup lang="ts">
</script>

<style lang="scss" scoped>
#index__contain {
  height: 100%;
  .main__wrap {
    width: 100%;
    display: flex;
    flex-direction: column;
    // border: 1px solid red;
  }
}
</style>