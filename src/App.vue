<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import TheMain from './components/TheMain.vue'
import CardContainer from './components/CardContainer.vue'
export default {
  components: {
    TheHeader,
    TheFooter,
    TheMain,
    CardContainer,
  }
}
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

<style></style>
