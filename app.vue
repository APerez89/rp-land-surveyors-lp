<template>
  <div class="app__contain">
    <NuxtLayout name="default">
      <div class="top__bar">
        <ContactBar />
      </div>
      <Nav />
      <NuxtPage />
      <Footer />
    </NuxtLayout>
  </div>
</template>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  border: 1px solid red;
}

:root {
  --max-width: 1300px;
}

.app__contain {
  width: 100%;
  min-height: 100vh;
  display: flex;
  justify-content: center;
}
</style>