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
    <packages />
    <occassions />
    <portofolios />
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'
import AppHeader from '~/components/AppHeader.vue'
import BookForm from '~/components/BookForm.vue'
import Portofolios from '~/components/Portofolios.vue'
import Occassions from '~/components/Occassions.vue'
import Packages from '~/components/Packages.vue'

export default {
  components: {
    Logo,
    VuetifyLogo,
    AppHeader,
    BookForm,
    Portofolios,
    Occassions,
    Packages
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
.app-row {
  display: -ms-flexbox; /* IE10 */
  display: flex;
  -ms-flex-wrap: wrap; /* IE10 */
  flex-wrap: wrap;
  margin: 0 -4px;
}
</style>
