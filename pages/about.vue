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
          <div class="team__contain">
            <div class="team__member">
              <div class="img__wrap">
                <img src="../public/richard_p.png" alt="">
              </div>
              <div class="text__wrap">
                <h3>Richard Plain Jr.</h3>
                <p>RichardPlain@email.com</p>
              </div>
            </div>
            <div class="team__member">
              <div class="img__wrap">
                <img src="../public/edward_p.png" alt="">
              </div>
              <div class="text__wrap">
                <h3>Edward Plain</h3>
                <p>EdwardPlain@email.com</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
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

        .team__contain {
          display: flex;
          justify-content: space-around;

          .team__member {
            display: flex;
            flex-direction: column;
            position: relative;
            // padding: 7px;
            background-color: var(--dark-blue);
            border-radius: 160px;
            transition: all 0.3s ease-in-out;

            .img__wrap {
              border-radius: 50%;
              position: relative;
              overflow: hidden;
              display: flex;
              box-shadow: 0px 6px 10px rgba(0,0,0,0.3);
              z-index: 1;
            }
            .text__wrap {
              height: calc(100% - 15px);
              display: flex;
              flex-direction: column;
              justify-content: flex-end;
              color: var(--light-white);
              position: absolute;
              padding: 50px;
              opacity: 0;
              transition: all 0.3s ease-in-out;
            }
          }
          .animate {
            background-color: var(--rp-red);
            padding-bottom: 150px;

            .text__wrap {
              opacity: 1;
            }
          }
        }
      }
    }
  }
}

</style>