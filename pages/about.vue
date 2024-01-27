<template>
  <section id="about" class="main__contain">
    <div class="about__wrap">
      <div class="about__t">
        <h4>About</h4>
        <h2>Richard W. Plain Land Surveying</h2>
      </div>
      
      <div class="about__b">
        <div class="about__b_t">
          <p>With over 70 years of combined experience Richard Plain, Jr. & Edward Plain make up the full service Survey Company - Richard Plain Land Surveyors, providing land surveys from mapping & staking to elevation certificates and more, all through Fairfield, New Haven and surrounding counties.</p>
          <br />
          <p>Established by our Father Richard and Uncle Edward Shaughnessy in 1978, The name "Richard Plain" remains a staple in Fairfield County. As a young boy, our Father Richard was taken under the wing of my Uncle Ed and decided that Land Surveying was his passion as well. They both worked together for over 50 years. Our Father has since retired and our Uncle passed away, but we proudly continue our family legacy. When you use our company, you are actually working directly with Richard & Edward! and we are honored to be the people on your project. We offer different types of surveys to satisfy different needs and we are here to direct you towards the type of survey that fits your situation (no more, no less) . With Richard W. Plain, you can be assured that the job will be done correctly and with a firm that has a great reputation!</p>
          <br />
          <p>We have the records of Shaughnessy & Plain, Land Surveyors, Fairfield and Edward G. Shaughnessy, Land Surveyor, Watertown, CT.</p>
        </div>
        <div class="about__b_b">
          <h2>Meet the Team</h2>
          <div class="img__contain">
            <div class="img__wrap">
              <img src="../public/richard_p.png" alt="">
              <div class="text__wrap">
                <p>Richard Plain</p>
                <p>RichardPlain@email.com</p>
              </div>
            </div>
            <div class="img__wrap">
              <img src="../public/edward_p.png" alt="">
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
definePageMeta ({
  layout: 'default'
})
</script>

<style lang="scss" scoped>
#about {
  width: 100%;
  padding: 60px 25px;
  font-family: 'Montserrat', sans-serif;
  .about__wrap {
    width: 100%;
    max-width: var(--max-width);

    .about__t {
      margin-bottom: 35px;

      h2 {
        font-size: 2.3rem;
        margin-bottom: 25px;
      }
      h4 {
        text-transform: uppercase;
        letter-spacing: 3px;
        font-size: 1rem;
        color: var(--rp-red);
      }
    }
    .about__b {
      .about__b_t {}
      .about__b_b {

        .img__contain {
          display: flex;
          .img__wrap {
            border-radius: 50%;
            position: relative;
            overflow: hidden;
            display: flex;
            box-shadow: 0px 6px 10px rgba(0,0,0,0.3);
            .text__wrap {
              width: 100%;
              height: 100%;
              border: 1px solid red;
              position: absolute;
              display: flex;
            }
          }
        }
      }
    }
  }
}
</style>