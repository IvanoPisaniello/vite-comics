<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import TheMain from './components/TheMain.vue'
import CardContainer from './components/CardContainer.vue'
import DcComics from '../src/dc-comics.json'
export default {
  components: {
    TheHeader,
    TheFooter,
    TheMain,
    CardContainer,





  },
  data() {
    return {
      cardList: DcComics,
    }
  }



}

console.log(DcComics)
</script>

<template>
  <header>
    <TheHeader></TheHeader>
  </header>
  <main>
    <TheMain></TheMain>
    <CardContainer></CardContainer>
  </main>
  <footer>
    <TheFooter></TheFooter>
  </footer>
</template>

<style>
body {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif
}
</style>
