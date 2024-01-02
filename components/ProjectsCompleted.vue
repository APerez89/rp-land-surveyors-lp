<template>
  <div id="projects__completed" class="main__contain">
    <div class="projects__wrap">
      <div class="projects__top">
        <h2>Recent Projects</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis quia vitae consequatur ad cupiditate possimus voluptatum quae quis. Fuga numquam aspernatur deserunt reprehenderit est quo iusto provident, dolores aut. Nisi?</p>
      </div>
      <div class="projects__bottom">
        <nuxt-link to="/" class="project__card">
          <div class="card__top">
            <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
          </div>
          <div class="card__bottom">
            <h4>448 Pequot Avenue</h4>
            <h4 class="location">Fairfield</h4>
            <div class="divider"></div>
            <p>The aim of this project was to create a "Zoning Location Survey" for some major renovation to an old house from 1834. Brian St. Pierre, a local Contractor that also hires us frequently, was in charge of this project.</p>
            
            <div class="animate">
              <h4>Learn More</h4>
            </div>
          </div>
        </nuxt-link>
        <nuxt-link to="/" class="project__card">
          <div class="card__top">
            <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
          </div>
          <div class="card__bottom">
            <h4>16 Orland Street</h4>
            <h4 class="location">Milford</h4>
            <div class="divider"></div>
            <p>The aim of the project was to create a "Zoning Location Survey" of existing conditions for Don & Susan so they can look at options for their garage. It is old, and had an old fashioned wood type floor, that cannot hold the weight of a car of today. </p>
            
            <div class="animate">
              <h4>Learn More</h4>
              <div class="card__icon">
                <svg fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M11.25 4.5l7.5 7.5-7.5 7.5m-6-15l7.5 7.5-7.5 7.5"></path>
                </svg>
              </div>
            </div>
          </div>
        </nuxt-link>
        <nuxt-link to="/" class="project__card">
          <div class="card__top">
            <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
          </div>
          <div class="card__bottom">
            <h4>116 Rowland Road</h4>
            <h4 class="location">Fairfield</h4>
            <div class="divider"></div>
            <p>The aim of this project was to create a "Zoning Location Survey" for proposal, for Luis & Mary Pat. As you can see, down by the beach, some towns require a great amount of detail on plans. They really do like to protect these areas as best they can.</p>
            
            <div class="animate">
              <h4>Learn More</h4>
            </div>
          </div>
        </nuxt-link>
        
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
#projects__completed {
  width: 100%;
  padding: 60px 25px;
  background: linear-gradient(
    to bottom,
    var(--light-white) 0%,
    var(--light-white) 70%,
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

    .projects__top {
      h2 {
        font-size: 2.3rem;
        margin-bottom: 25px;
      }
    }
    .projects__bottom {
      width: 100%;
      display: grid;
      gap: 25px;
      grid-template-columns: repeat(3, 1fr);
      justify-content: center;
      margin: 25px 0px;
      
      .project__card {
        width: 100%;
        max-width: 350px;
        background-color: var(--light-white);
        position: relative;
        border-radius: 8px;
        overflow: hidden;
        text-decoration: none;
        color: var(--dark-blue);
        box-shadow: 0px 15px 15px -4px rgba(0,0,0,0.4);
        transition: all 0.2s ease-in-out;

        .card__top {
          img {
            width: 100%;
          }
        }

        .card__bottom {
          padding: 15px;

          h4 {
            font-size: 1.4rem;
            font-weight: 600;
            // padding-bottom: 10px;
            // margin-bottom: 15px;
            letter-spacing: 1px;
            // border-bottom: 2px solid var(--rp-red);
          }
          
          .location {
            font-size: 1rem;
            font-weight: 500;
            text-transform: uppercase;
            color: var(--dark-gray);
            // font-style: italic;
            margin-top: 8px;
          }

          .divider {
            width: 15%;
            height: 2px;
            background-color: var(--rp-red);
            margin: 15px 0px;
          }

          p {
            color: var(--dark-gray);
            letter-spacing: 1px;
            line-height: 25px;
          }
        }

        .animate {
          display: flex;
          justify-content: end;
          position: relative;
          margin-top: 15px;
          transform: translateX(15px);
          text-decoration: underline;
          opacity: 0;
          transition: all 0.2s ease-in-out;

          h4 {
            font-size: 1rem;
          }

          .card__icon {
            width: 20px;
            color: var(--dark-blue);
            margin-left: 6px;
          }
        }

        &:hover {
          transform: translateY(-5px);
          box-shadow: 0px 20px 15px -8px rgba(0,0,0,0.4);

          .animate {
            transform: translateX(0px);
            opacity: 1;
          }
        }
      }
    }
  }
}
</style>