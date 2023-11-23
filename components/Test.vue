<template>
  <div id="test__contain" class="main__contain">
    <div class="test__wrap">
      <h2>test test test</h2>
      <div class="img__wrap">
        <img src="../public/theodolite.png" alt="AI generated image of a thedolite.">
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#test__contain {
  width: 100%;
  height: 100%;
  background-color: var(--off-white);

  .test__wrap {
    max-width: var(--max-width);
    width: 100%;
  }
  .img__wrap {
    width: 100%;
    position: relative;
    img {
      transform: rotate(15deg);
    }
  }
}
</style>