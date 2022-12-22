<script>
import InfoCompany from './components/Header/InfoCompany.vue'
import Jumbotron from './components/Header/Jumbotron.vue'
import AppMain from './components/Main/AppMain.vue'
import AppFooter from './components/Footer/AppFooter.vue'

export default {
  name: "App",
  components: {
    InfoCompany,
    Jumbotron,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <header>
    <InfoCompany />
    <Jumbotron />
  </header>

  <AppMain />

  <AppFooter />

</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
