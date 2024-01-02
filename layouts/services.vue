<template>
  <div class="services__contain">
    <Nav />
    <div class="content">
      <slot />
    </div>
    <Footer />
  </div>
</template>

<style lang="scss" scoped>
.services__contain {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  font-family: 'Raleway', sans-serif;
  background-color: var(--light-white);
  overflow: hidden;

  .content {
    flex-grow: 1;
  }
}
</style>