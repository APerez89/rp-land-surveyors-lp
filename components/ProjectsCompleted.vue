<script setup src="">
import data from '../composables/rpData';

const projects = data.projects;
const highlighted = [];

const findHighlight = () => {
  projects.forEach((project) => {
    if(project.highlight === true) {
      highlighted.push(project);
    }
  })
}
findHighlight();
</script>

<template>
  <div id="projects__completed" class="main__contain">
    <div class="projects__wrap">
      <div class="projects__top">
        <h4>Our</h4>
        <h2>Featured Projects</h2>
        <Divider />
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis quia vitae consequatur ad cupiditate possimus voluptatum quae quis. Fuga numquam aspernatur deserunt reprehenderit est quo iusto provident, dolores aut. Nisi?</p>
      </div>
      <div class="projects__bottom">
        <HighlightCard v-for="(card, index) in highlighted" :key="index" :data="card" />
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
#projects__completed {
  width: 100%;
  padding: 60px 25px;
  font-family: 'Montserrat', sans-serif;
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
    .projects__bottom {
      width: 100%;
      display: grid;
      gap: 25px;
      grid-template-columns: repeat(3, 1fr);
      justify-items: center;
      margin: 25px 0px;
    }
  }
}
</style>