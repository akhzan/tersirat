<template>
  <div class="occassions">
    <div class="occassions__title">Occassions</div>
    <div class="app-row">
      <div class="occassions__column">
        <v-img src="https://cdn.sweetescape.com/misc/home/occasions/img-honeymoon.jpg" style="width:100%" />
        <div class="occassions__column-title">Prewedding</div>
      </div>
      <div class="occassions__column">
        <v-img src="https://cdn.sweetescape.com/misc/home/occasions/img-honeymoon.jpg" style="width:100%" />
        <div class="occassions__column-title">Engagement</div>
      </div>
      <div class="occassions__column">
        <v-img src="https://cdn.sweetescape.com/misc/home/occasions/img-honeymoon.jpg" style="width:100%" />
        <div class="occassions__column-title">Akad</div>
      </div>
      <div class="occassions__column">
        <v-img src="https://cdn.sweetescape.com/misc/home/occasions/img-honeymoon.jpg" style="width:100%" />
        <div class="occassions__column-title">Pengajian</div>
      </div>
      <div class="occassions__column">
        <v-img src="https://cdn.sweetescape.com/misc/home/occasions/img-honeymoon.jpg" style="width:100%" />
        <div class="occassions__column-title">Siraman</div>
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
.occassions {
  width: 80%;
  margin-top: 2em;
  text-align: left;
  .occassions__title {
    font-size: 1.5rem;
    font-weight: bold;
  }
  .app-row {
    margin: 0 -8px !important;
  }
}
.occassions__column {
  -ms-flex: 20%; /* IE10 */
  flex: 20%;
  max-width: 20%;
  padding: 0 8px;
  div {
    margin-top: 8px;
    vertical-align: middle;
  }
}
.occassions__column-title {
  text-transform: uppercase;
}
</style>
