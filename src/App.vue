<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import Card from './components/Card.vue'
import MenuContainer from './components/MenuContainer.vue'
import Cards from '../src/mydatabase/cards'
import Hero from '../src/components/Hero.vue'
export default {
  components: {
    TheHeader,
    TheFooter,
    Card,
    MenuContainer,
    Cards,
    Hero,






  },
  data() {
    return {
      Cards
    }
  }



}

console.log(Cards)
</script>

<template>
  <header>
    <TheHeader></TheHeader>
  </header>
  <main>
    <div class="jumbo-container">
      <Hero></Hero>

    </div>
    <div class="d-flex justify-content-center pb-3 hero-btn">
      <button class="btn btn-primary px-4 rounded-0">
        CURRENT SERIES
      </button>
    </div>
    <div class="d-flex flex-wrap gap-4 container card-container p-3">

      <Card :thumb="card.thumb" :series="card.series" v-for="(card, i) in Cards" class="single-card" :key="singleCard">
      </Card>

    </div>
    <div class="d-flex justify-content-center pb-3">
      <button class="btn btn-primary px-4 py-0 rounded-0">
        LOAD MORE
      </button>
    </div>
    <MenuContainer></MenuContainer>
  </main>
  <footer>
    <TheFooter></TheFooter>
  </footer>
</template>

<style lang="scss">
@use "./styles/partials/variables" as *;

body {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif
}

main {
  background-color: $color-secondary;
  position: relative;

  .jumbo-container {
    height: 300px;
    overflow: hidden;
    position: relative;
  }

  p {
    font-size: .7rem;
  }


}

.card-container {

  width: 800px;


  .single-card {
    width: 100px;


  }



}

.hero-btn {
  position: absolute;
  left: 23%;
  top: 29%;


}
</style>
