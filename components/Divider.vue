<template>
  <div id="divider" class="main__contain">
    <div class="divider__wrap">
      <h4><q><i>The homeowner doesn't know what we do, it is our job to <span class="highlight">educate</span> them.</i></q></h4>
      <h4 class="rps">- Richard Plain, Sr.</h4>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#divider {
  background-color: var(--not-black);
  padding: 25px;
  z-index: 10;
  .divider__wrap {
    display: flex;
    flex-direction: column;
    color: var(--light-white);

    h4 {
      font-size: 1.6rem;
      font-weight: 200;
    }

    .rps {
      align-self: flex-end;
      margin-top: 15px;
    }
  }
}
</style>