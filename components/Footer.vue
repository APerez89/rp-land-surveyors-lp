<script setup lang="ts">
const getYear = new Date().getFullYear();
</script>

<template>
  <footer id="footer" class="main__contain">
    <div class="footer__wrap">
      <div class="footer__content">
        <div class="logo__wrap">
          <img src="../public/footer-logo.png" alt="Richard Plain Footer Logo">
        </div>
        <div class="copy">
          <p>&copy; {{ getYear }}. All Rights Reserved</p>
        </div>
        <div class="footer__bottom">
          <nuxt-link to="privacy">Privacy Policy</nuxt-link>
          <div class="divider"></div>
          <nuxt-link to="https://www.facebook.com/richardplainsurveyors" target="__blank">Facebook</nuxt-link>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
#footer {
  background-color: var(--dark-blue);
  color: var(--light-white);

  .footer__wrap {
    width: 100%;
    max-width: var(--max-width);
    justify-content: center;
    padding: 45px;

    .footer__content {
      width: 100%;
      display: grid;
      gap: 20px;
      text-align: center;

      .footer__bottom {
        display: flex;
        justify-content: center;

        a {
          text-decoration: none;
          color: var(--light-white);

          &:hover {
            text-decoration: underline;
          }
        }
        .divider {
          width: 1px;
          height: 100%;
          background-color: var(--light-white);
          margin: 0px 15px;
        }
      }
    }
  }
}
</style>