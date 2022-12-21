<script>
import InfoCompany from './components/InfoCompany.vue'
import Jumbotron from './components/Jumbotron.vue'

export default {
  name: "App",
  components: {
    InfoCompany,
    Jumbotron
  }
}
</script>

<template>
  <header>

    <InfoCompany />
    <Jumbotron />

  </header>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
