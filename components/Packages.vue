<template>
  <div class="packages">
    <div class="packages__title">Packages</div>
    <div class="app-row">
      <div class="packages__column">
        <div class="packages__item">
          <div class="package__item-title">
            <h5>PHOTOGRAPHY</h5>
            <div><b>IDR 1200 K</b> / session</div>
          </div>
          <div class="package__item-action">
            <a>see detail</a>
          </div>
        </div>
      </div>
      <div class="packages__column">
        <div class="packages__item">
          <div class="package__item-title">
            <h5>PHOTO & VIDEO</h5>
            <div><b>IDR 800 K</b> / session</div>
          </div>
          <div class="package__item-action">
            <a>see detail</a>
          </div>
        </div>
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
  .app-row {
    margin: 1em -8px 0 -8px !important;
  }
}
.packages__column {
  -ms-flex: 50%; /* IE10 */
  flex: 50%;
  max-width: 50%;
  padding: 0 8px;
}
.packages__item {
  padding: 1em 1.5em;
  background-color: white;
  // color: white;
  box-shadow: rgba(0, 0, 0, 0.06) 0px 2px 4px 0px !important;
  height: 100%;
}
.package__item-title {
  display: flex;
  justify-content: space-between;
  align-items: center;
  h5 {
    font-size: 1.5rem;
    font-weight: normal;
  }
}
.package__item-action {
  text-align: right;
  a {
    color: rgb(0, 170, 255);
  }
}
</style>
