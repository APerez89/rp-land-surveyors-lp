<script setup lang="ts">
</script>

<template>
  <nav id="nav" class="main__contain">
    <div class="nav__wrap">
      <div class="logo__wrap">
        <nuxt-link to="/">
          <img src="main-logo-small.webp" alt="">
        </nuxt-link>
      </div>
      <div class="right__nav">
        <div class="nav__contact">
          <div class="location__wrap">
            <h5>
              <div class="pin icon">
                <svg fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                  <path clip-rule="evenodd" fill-rule="evenodd" d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"></path>
                </svg>
              </div>
              <nuxt-link
                href="https://maps.app.goo.gl/FbGDrxqqycmP26HM6"
                target="_blank"
              >
                29 Hunters Rn Rd, Milford, CT 06460
              </nuxt-link>
            </h5>
          </div>
          <div class="phone__wrap">
            <h5>
              <div class="phone icon">
                <svg fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                  <path clip-rule="evenodd" fill-rule="evenodd" d="M1.5 4.5a3 3 0 013-3h1.372c.86 0 1.61.586 1.819 1.42l1.105 4.423a1.875 1.875 0 01-.694 1.955l-1.293.97c-.135.101-.164.249-.126.352a11.285 11.285 0 006.697 6.697c.103.038.25.009.352-.126l.97-1.293a1.875 1.875 0 011.955-.694l4.423 1.105c.834.209 1.42.959 1.42 1.82V19.5a3 3 0 01-3 3h-2.25C8.552 22.5 1.5 15.448 1.5 6.75V4.5z"></path>
                </svg>
              </div>
              <nuxt-link href="tel:2038783818">
                203.878.3818
              </nuxt-link>
            </h5>
          </div>
        </div>
        <div class="nav__items">
          <div class="item">
            <nuxt-link to="about">About</nuxt-link>
          </div>
          <div class="item">
            <nuxt-link to="services" class="services">
              Services
              <div class="icon">
                <svg fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                  <path clip-rule="evenodd" fill-rule="evenodd" d="M12.53 16.28a.75.75 0 01-1.06 0l-7.5-7.5a.75.75 0 011.06-1.06L12 14.69l6.97-6.97a.75.75 0 111.06 1.06l-7.5 7.5z"></path>
                </svg>
              </div>
            </nuxt-link>
          </div>
          <div class="item">
            <nuxt-link to="projects">Projects</nuxt-link>
          </div>
          <div class="item">
            <nuxt-link to="contact">Contact</nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@200;300;400;600&display=swap');

#nav {
  font-family: 'Raleway', sans-serif;

  a {
    color: var(--gray);
    letter-spacing: 1px;
    // font-weight: 400;
  }
  
  .icon {
    width: 17px;
    display: flex;
    align-items: center;
    margin-right: 7px;
    color: var(--gray);
  }

  h5 {
    display: flex;
    align-items: center;
    letter-spacing: 1px;
  }

  .nav__wrap {
    width: 100%;
    display: flex;
    max-width: var(--max-width);
    justify-content: space-between;
    padding: 10px 0px;

    .right__nav {
      display: inline-flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: flex-end;

      .location__wrap {
        margin-right: 20px;
      }

      .nav__contact {
        display: flex;
        // padding-bottom: 10px;
      }
      .nav__items {
        display: inline-flex;
        align-items: flex-end;
        // border: 1px solid red;
  
        .item {
          display: contents;
  
          a {
            padding: 10px 25px;
            text-decoration: none;
          }

          .services {
            display: inline-flex;

            .icon {
              margin: 0px 0px 0px 10px;
            }
          }
        }
      }
    }
  }
}
</style>