<script setup>
const props = defineProps({
  data: Object,
})

</script>

<template>
  <div id="card__highlight" class="card__contain">
    <nuxt-link :to="`projects/${data.slug}`" class="proj__card">
      <div class="card__t">
        <img src="../public/land-surveying.png" alt="AI Generated Theodolite on a tripod">
      </div>
      <div class="card__b">
        <div class="card__info">
          <h4>{{ data.address }}</h4>
          <h4 class="city">{{ data.city }}</h4>
          <div class="divider"></div>
          <p>{{ data.text }}</p>
        </div>
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
  </div>
</template>

<style lang="scss" scoped>
.card__contain {
  display: flex;

  .proj__card {
    width: 100%;
    max-width: 350px;
    display: flex;
    flex-direction: column;
    background-color: var(--light-white);
    position: relative;
    border-radius: 8px;
    overflow: hidden;
    text-decoration: none;
    color: var(--dark-blue);
    box-shadow: 0px 8px 15px -4px rgba(0,0,0,0.4);
    transition: all 0.2s ease-in-out;
  
    .card__t {
      img {
        width: 100%;
      }
    }
  
    .card__b {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      flex-grow: 1;
      padding: 15px;

      .card__info {
        
        h4 {
          font-size: 1.4rem;
          font-weight: 600;
          letter-spacing: 1px;
        }
        
        .city {
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
</style>