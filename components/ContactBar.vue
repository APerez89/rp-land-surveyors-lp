<template>
  <section id="contact__bar" class="main__contain">
    <div class="contact__bar_wrap">
      <div>
        <h4>
          <a
            href="https://maps.app.goo.gl/FbGDrxqqycmP26HM6"
            target="_blank"
          >
            29 Hunters Rn Rd, Milford, CT 06460
          </a>
        </h4>
      </div>
      <div class="phone__wrap">
        <h4>
          <a href="tel:2038783818">
            203.878.3818
          </a>
        </h4>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
#contact__bar {
  background-color: var(--rp-black);
  .contact__bar_wrap {
    width: 100%;
    max-width: var(--max-width);
    display: flex;
    justify-content: space-between;
    padding: 10px 0px;

    a {
      color: var(--off-white);
      text-decoration: none;
    }
  }
}
</style>