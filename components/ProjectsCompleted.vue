<template>
  <div id="projects__completed" class="main__contain">
    <div class="projects__wrap">
      <div class="projects__left">
        <h2>Recent Projects</h2>
      </div>
      <div class="projects__right">
        <div class="project__card">
          <div class="card__top">
            <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
          </div>
          <div class="card__bottom"></div>
        </div>
        <div class="project__card">
          <div class="card__top">
            <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
          </div>
          <div class="card__bottom"></div>
        </div>
        <div class="project__card">
          <div class="card__top">
            <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
          </div>
          <div class="card__bottom"></div>
        </div>
        
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
#projects__completed {
  width: 100%;
  padding: 25px;
  background: linear-gradient(
    to bottom,
    var(--off-white) 0%,
    var(--off-white) 70%,
    var(--rp-red) 70%,
    var(--rp-red) 100%
  );
  .projects__wrap {
    width: 100%;
    max-width: var(--max-width);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .projects__left {
      h2 {
        font-size: 2.3rem;
        margin-bottom: 25px;
      }
    }
    .projects__right {
      width: 100%;
      display: grid;
      gap: 25px;
      grid-template-columns: repeat(3, 350px);
      justify-content: center;
      margin: 25px 0px;
      
      .project__card {
        width: 100%;
        max-width: 350px;
        background-color: var(--off-white);
        border-radius: 8px;
        overflow: hidden;
        box-shadow: 0px 23px 15px -11px rgba(0,0,0,0.4);

        .card__top {
          img {
            width: 100%;
          }
        }

        .card__bottom {
          padding: 15px;
        }
      }
    }
  }
}
</style>