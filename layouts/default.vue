<template>
  <v-app>
    <v-content>
      <nuxt />
    </v-content>
    <v-footer class="footer">
      <span class="footer__copy">&copy; 2018. Tersirat. All rights Reserved.</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        { icon: 'apps', title: 'Welcome', to: '/' },
        { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>

<style lang="scss">
.footer {
  margin-top: 20px;
}
.footer__copy {
  padding: 0 40px;
  font-size: 1rem;
}
</style>
