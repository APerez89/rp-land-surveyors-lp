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

  .app_wrap {
    display: flex;
    position: relative;
  }
}
</style>