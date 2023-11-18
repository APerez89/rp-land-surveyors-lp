<template>
  <div class="app__contain">
    <NuxtLayout name="default" class="default">
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
  border: 1px solid red;
}

:root {
  --max-width: 1300px;
}
</style>