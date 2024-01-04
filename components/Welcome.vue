<script setup lang="ts">
import data from '../composables/rpData';

const serviceList = data.services;

</script>

<template>
  <div id="welcome__contain" class="main__contain">
    <div class="welcome__wrap">
      <div class="welcome__info">
        <div class="info__wrap">
          <h4>Since 1978</h4>
          <h1>Richard W. Plain</h1>
          <h2>Land Surveyors</h2>
        </div>
        <div class="divider"></div>
        <div class="services__wrap">
          <div class="services" v-for="(service, index) in serviceList" :key="index">
            <p>{{ service.title }}</p>
          </div>
        </div>
        <!-- <div class="divider"></div> -->
        <Button link="contact" message="Contact" />
      </div>
      <div class="img__wrap">
        <div class="dark__bkg"></div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#welcome__contain {
  .welcome__wrap {
    width: 100%;
    height: 1000px;
    padding: 50px 25px;
    max-width: var(--max-width);
    display: grid;
    grid-template-columns: 1fr 1fr;
    .welcome__info {
      display: flex;
      flex-direction: column;
      justify-content: center;
      font-family: 'Montserrat', sans-serif;
      color: var(--not-black);

      .info__wrap {

        h1 {
          font-size: 4rem;
          font-weight: 700;
        }
  
        h2 {
          color: var(--gray);
          font-weight: 300;
          letter-spacing: 2px;
        }
  
        h4 {
          text-transform: uppercase;
          letter-spacing: 3px;
          font-size: .8rem;
          color: var(--rp-red);
        }
      }

      .divider {
        width: 100%;
        height: 2px;
        background-color: var(--rp-red);
        margin: 20px 0px;
      }

      .services__wrap {
        width: 100%;
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 15px;
        margin-bottom: 15px;

        .services {
          padding: 10px 15px;
          position: relative;
          font-family: 'Raleway', sans-serif;
          font-weight: 400;
          letter-spacing: 1px;

          &::before {
            content: '';
            position: absolute;
            top: 45%;
            right: 0;
            bottom: 0;
            left: 0;
            width: 5px;
            height: 5px;
            background-color: var(--rp-red);
            border-radius: 50%;
          }
        }
      }

    }
    .img__wrap {
      position: relative;
      background-image: url('../public/richard_plain.png');
      background-size: cover;
      background-position: 50%;
      background-repeat: no-repeat;
      overflow: hidden;

      .dark__bkg {
        width: 100%;
        height: 100%;
        background-color: rgba(0,0,0,0.4);
      }
    }

    .img__wrap::before {
      content: '';
      position: absolute;
      transform: translate(-50%, -10%) rotate(5deg);
      background: var(--light-white);
      width: 20%;
      height: 140%;
    }
  }
}
</style>