<template>
  <div class="app__contain">
    <NuxtLayout name="default" class="app__wrap">
      <ContactBar />
      <Nav />
      <NuxtPage />
      <Footer />
    </NuxtLayout>
  </div>
</template>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
}

:root {
  --max-width: 1300px;
  --rp-red: #ec2c2c;
  --rp-black: #232323;
  --off-white: #efeff1;
  --light-white: #f6f6f6;
}

.main__contain {
  width: 100%;
  display: flex;
  justify-content: center;
  border: 1px solid red;
}

.app__contain {
  min-height: 100vh;
  border: 1px solid red;
  background-color: var(--light-white);

  .app_wrap {
    display: flex;
    position: relative;
  }
}
</style>