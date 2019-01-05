<template>
  <div class="packages">
    <div class="packages__title">Packages</div>
    <div class="app-row">
      <div class="packages__column">
        <v-img src="https://picsum.photos/500/300?image=15" style="width:100%" />
      </div>
      <div class="packages__column">
        <v-img src="https://picsum.photos/500/300?image=15" style="width:100%" />
      </div>
    </div>
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
.packages {
  width: 80%;
  margin-top: 2em;
  text-align: left;
  .packages__title {
    font-size: 1.5rem;
    font-weight: bold;
  }
}
.packages__column {
  -ms-flex: 50%; /* IE10 */
  flex: 50%;
  max-width: 50%;
  padding: 0 8px;
  div {
    margin-top: 8px;
    vertical-align: middle;
  }
}
</style>
