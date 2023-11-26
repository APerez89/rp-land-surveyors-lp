<template>
  <div id="projects__completed">
    <div class="main__contain backdrop-blur">
      <div class="projects__wrap">
        <div class="projects">
          <h4>Projects Completed</h4>
        </div>
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
#projects__completed {
  width: 100%;
  min-height: 1000px;
  background-image: url('../public/land-surveying.png');
  background-size: cover;
  background-position: 50%;
  background-repeat: no-repeat;

  .backdrop-blur {
    height: 100%;
    background: transparent;
    backdrop-filter: blur(4px);
    background-color: rgba(235,46,46,.25);
    z-index: 1;

    .projects__wrap {
      width: 100%;
      max-width: var(--max-width);
    }
  }
}
</style>