<template>
  <div class="app__contain">
      <!-- <ContactBar /> -->
      <Nav />
      <slot />
      <Footer />
         <!-- Youtube Link -->
         <!-- 
          <iframe width="560" height="315" src="https://www.youtube.com/embed/RP7C6278zp0?si=EQ0dxNXipuclTkLj&amp;controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          -->
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@200;300;400;600&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500;700&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
}

:root {
  --max-width: 1300px;
  --rp-red: #ec2c2c;
  --rp-light-red: #e74949;
  --not-black: #232323;
  --off-white: #efeff1;
  --light-white: #f6f6f6;
  --gray: #939393;
  --dark-gray: #717171;
}

.main__contain {
  width: 100%;
  display: flex;
  justify-content: center;
  // border: 1px solid red;
}

.highlight {
  color: var(--rp-red);
}

.app__contain {
  min-height: 100vh;
  font-family: 'Raleway', sans-serif;
  background-color: var(--light-white);
  overflow: hidden;

  .app_wrap {
    display: flex;
    position: relative;
  }
}
</style>