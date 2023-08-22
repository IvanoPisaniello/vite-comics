<script>
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
import TheMain from './components/TheMain.vue'
export default {
  components: {
    TheHeader,
    TheFooter,
    TheMain,
  }
}
</script>

<template>
  <header>
    <TheHeader></TheHeader>
  </header>
  <main>
    <TheMain></TheMain>
  </main>
</template>

<style></style>
