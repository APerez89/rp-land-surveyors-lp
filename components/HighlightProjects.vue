<template>
  <div id="projects__completed" class="main__contain">
    <div class="projects__wrap">
      <div class="projects__top">
        <h2>Project Highlights</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis quia vitae consequatur ad cupiditate possimus voluptatum quae quis. Fuga numquam aspernatur deserunt reprehenderit est quo iusto provident, dolores aut. Nisi?</p>
      </div>
      <div class="projects__bottom">
        <nuxt-link to="/" class="project__card">
          <div class="overlay"></div>
          <div class="card__top">
            <div class="top__detail">
              <h4>Southport Expansion</h4>
            </div>
            <div class="mid__detail">
              <h4>448 Pequot Avenue</h4>
              <h4 class="location">Fairfield</h4>
            </div>
            <div class="bot__detail">
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
          <div class="overlay"></div>
          <div class="card__top">
            <div class="top__detail">
              <h4>Addressing The Garage</h4>
            </div>
            <div class="mid__detail">
              <h4>16 Orland Street</h4>
              <h4 class="location">Milford</h4>
            </div>
            <div class="bot__detail">
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
          <div class="overlay"></div>
          <div class="card__top">
            <div class="top__detail">
              <h4>A Small Addition</h4>
            </div>
            <div class="mid__detail">
              <h4>116 Rowland Road</h4>
              <h4 class="location">Fairfield</h4>
            </div>
            <div class="bot__detail">
              <h4>Learn More</h4>
              <div class="card__icon">
                <svg fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M11.25 4.5l7.5 7.5-7.5 7.5m-6-15l7.5 7.5-7.5 7.5"></path>
                </svg>
              </div>
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
  background-color: var(--light-white);
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
        background-image: url('../public/land-surveying.png');
        background-size: cover;
        background-position: 50%;
        background-repeat: no-repeat;
        position: relative;
        text-decoration: none;
        color: var(--off-white);
        box-shadow: 0px 0px 15px rgba(0,0,0,0.4);
        overflow: hidden;
        transition: all 0.2s ease-in-out;

        .overlay {
          width: 100%;
          height: 100%;
          background-color: var(--dark-blue);
          opacity: 0.6;
          position: absolute;
          transition: all 0.2s ease-in-out;
          z-index: 1;
        }

        .card__top {
          height: 100%;
          min-height: 400px;
          display: flex;
          flex-direction: column;
          justify-content: space-between;
          text-align: center;
          padding: 25px;
          position: inherit;
          color: var(--light-white);
          z-index: 2;

          h4 {
            text-shadow: 0px 0px 10px rgba(0,0,0,0.6);
          }

          .top__detail {
            position: relative;
            transform: translateY(-15px);
            opacity: 0;
            transition: all 0.2s ease-in-out;

            h4 {
              font-size: 1.1rem;
              letter-spacing: 1.1px;
              text-transform: uppercase;
              font-weight: 500;
            }
          }

          .mid__detail {
            h4 {
              font-size: 1.4rem;
              font-weight: 600;
              letter-spacing: 1px;
            }
            .location {
              font-size: 1rem;
              font-weight: 500;
              letter-spacing: 1.1px;
              text-transform: uppercase;
              margin-top: 8px;
            }
          }

          .bot__detail {
            display: flex;
            justify-content: center;
            position: relative;
            transform: translateY(15px);
            opacity: 0;
            transition: all 0.2s ease-in-out;
            
            h4 {
              letter-spacing: 1px;
              font-size: 1rem;
              text-decoration: underline;
            }

            .card__icon {
              width: 20px;
              // color: var(--dark-blue);
              margin-left: 6px;
            }
          }
        }
        
        &:hover {
          transform: scale(1.01);
          box-shadow: 0px 20px 15px -8px rgba(0,0,0,0.4);
          z-index: 2;

          .overlay {
            background-color: var(--rp-red);
          }

          .top__detail, .bot__detail {
            transform: translateX(0px);
            opacity: 1;
          }
        }
      }
    }
  }
}
</style>