<template>
  <div id="projects__completed" class="main__contain">
    <div class="projects__wrap">
      <div class="projects__left">
        <h4>Projects Completed</h4>
      </div>
      <div class="projects__right">
        <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
#projects__completed {
  width: 100%;
  .projects__wrap {
    width: 100%;
    max-width: var(--max-width);
    display: flex;

    .projects__left {}
    .projects__right {
      width: 50%;
      img {
        width: 100%;
      }
    }
  }
}
</style>