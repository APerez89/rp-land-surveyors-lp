<template>
  <div id="why__contain" class="main__contain">
    <div class="why__wrap">
      <div class="img__wrap">
        <img src="../public/theodolite.png" alt="AI generated image of a thedolite.">
      </div>
      <div class="why__info">
        <h4>Why</h4>
        <h2>Richard Plain Land Surveyors</h2>
        <div class="copy">
          <p>With over 70 years of combined experience Richard Plain, Jr. & Edward Plain make up the <span class="highlight">Full Service Survey Company</span> - Richard Plain Land Surveyors, providing land surveys from mapping & staking to elevation certificates and more, all through Fairfield, New Haven and surrounding counties.</p>
        </div>
        <div class="button">
          <Button link="about" message="Learn More" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#why__contain {
  background-color: var(--off-white);
  font-family: 'Montserrat', sans-serif;

  .why__wrap {
    max-width: var(--max-width);
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 25px;

    .img__wrap {
      width: 100%;
      position: relative;

      img {
        width: 130%;
        position: inherit;
        transform: rotateY(180deg) rotate(15deg);
        left: -150px;
      }
    }

    .why__info {
      width: 100%;
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;

      h2 {
        font-size: 2.3rem;
        color: var(--not-black);
        letter-spacing: 3px;
        padding-bottom: 15px;
        border-bottom: 2px solid var(--rp-red);
      }
      
      h4 {
        text-transform: uppercase;
        letter-spacing: 3px;
        font-size: 1rem;
        color: var(--rp-red);
      }

      .copy {
        margin-top: 25px;

        p {
          font-family: 'Raleway', sans-serif;
          font-size: 1.3rem;
          color: var(--gray);
          letter-spacing: 1.1px;
          line-height: 38px;
        }
      }

      .button {
        width: 100%;
        display: flex;
        justify-content: flex-end;
      }
    }
  }
}
</style>