<script>
import InfoCompany from './components/Header/InfoCompany.vue'
import Jumbotron from './components/Header/Jumbotron.vue'
import AppMain from './components/AppMain.vue'

export default {
  name: "App",
  components: {
    InfoCompany,
    Jumbotron,
    AppMain
  }
}
</script>

<template>
  <header>
    <InfoCompany />
    <Jumbotron />
  </header>

  <AppMain />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
