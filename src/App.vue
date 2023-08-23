<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import Card from './components/Card.vue'
import MenuContainer from './components/MenuContainer.vue'
import Cards from '../src/mydatabase/cards'
export default {
  components: {
    TheHeader,
    TheFooter,
    Card,
    MenuContainer,
    Cards,






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
    <div class="d-flex flex-wrap gap-4 container card-container">
      <Card :img-src="card.thumb" v-for="(card, i) in Cards" class="single-card"></Card>
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
}

.card-container {

  width: 800px;


  .single-card {
    width: 100px;
  }

}
</style>
