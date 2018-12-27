<template>
  <v-layout
    class="home-layout"
    column
    justify-center
    align-center>
    <div class="home-book">
      <app-header />
      <book-form />
    </div>
    <covered-events />
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'
import AppHeader from '~/components/AppHeader.vue'
import BookForm from '~/components/BookForm.vue'
import CoveredEvents from '~/components/CoveredEvents.vue'

export default {
  components: {
    Logo,
    VuetifyLogo,
    AppHeader,
    BookForm,
    CoveredEvents
  }
}
</script>

<style lang="scss">
html {
  margin: 0;
  padding: 0;
  font-size: 10px;
}
body {
  margin: 0;
  padding: 0;
  font-size: 1.2rem;
}
.home-book {
  height: 100vh;
  width: 100vw;
  background-image: url('~assets/back.jpg');
  background-size: cover;
}
</style>
