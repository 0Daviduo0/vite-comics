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
  },
  data(){
    return{
            AppHeaderLogo: '../../src/assets/dc-logo.png',
            AppHeaderLinks: [
            {
                text: "CHARACTERS",
                url: "",
                current: false,
            },
            {
                text: "COMICS",
                url: "",
                current: true,
            },
            {
                text: "MOVIES",
                url: "",
                current: false,
            },
            {
                text: "TV",
                url: "",
                current: false,
            },
            {
                text: "GAMES",
                url: "",
                current: false,
            },
            {
                text: "VIDEOS",
                url: "",
                current: false,
            },
            {
                text: "FANS",
                url: "",
                current: false,
            },
            {
                text: "NEWS",
                url: "",
                current: false,
            },
            {
                text: "SHOP",
                url: "",
                current: false,
            },
            ],
            AppMainComponents: [
            {
                image: "../../src/assets/buy-comics-digital-comics.png",
                text: "DIGITAL COMICS",
            },
            {
                image: "../../src/assets/buy-comics-merchandise.png",
                text: "DC MERCHANDISE",
            },
            {
                image: "../../src/assets/buy-comics-subscriptions.png",
                text: "SUBSCRIPTION",
            },
            {
                image: "../../src/assets/buy-comics-shop-locator.png",
                text: "COMIC SHOP LOCATOR",
            },
            {
                image: "../../src/assets/buy-dc-power-visa.svg",
                text: "DC POWER VISA",
            },
            ],
    }
    
  }
}
</script>

<template>
  <header>
    <AppHeader :logo="AppHeaderLogo" :links="AppHeaderLinks"/>
  </header>
  <main>
    <AppMain :components="AppMainComponents"/>
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
