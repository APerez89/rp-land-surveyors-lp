<template>
  <footer id="footer" class="main__contain">
    <div class="footer__wrap">
      <div class="footer__content">
        <h2>
          SugarFooter
        </h2>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
#footer {
  height: 150px;
  background-color: #0e111a;
  color: #e7e7e7;
  border: 1px solid red;

  .footer__wrap {
    width: 100%;
    max-width: var(--max-width);
    justify-content: center;

    .footer__content {
      border: 1px solid red;
    }
  }
}
</style>