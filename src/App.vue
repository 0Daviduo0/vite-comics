<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: "app",
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <header>
    <AppHeader/>
  </header>
  <main>
    <AppMain/>
  </main>
  <footer>
    <AppFooter/>
  </footer>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;
@use './styles/partials/mixins' as *;
@use './styles/general.scss' as *;
</style>
