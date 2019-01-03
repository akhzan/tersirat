<template>
  <div class="portofolios">
    <div class="portofolios__title">Portofolios</div>
    <photo-grid />
  </div>
</template>

<script>
import PhotoGrid from '~/components/PhotoGrid.vue'

export default {
  components: {
    PhotoGrid
  }
}
</script>


<style lang="scss">
.portofolios {
  width: 80%;
  margin-top: 2em;
  text-align: left;
  .portofolios__title {
    font-size: 1.5rem;
    margin-bottom: 1em;
    font-weight: bold;
  }
}
</style>
