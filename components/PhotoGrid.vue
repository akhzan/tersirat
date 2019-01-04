<template>
  <div class="app-row">
    <div class="photo-grid__column">
      <v-img src="https://picsum.photos/500/300?image=15" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=16" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=17" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=18" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=19" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=20" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=21" style="width:100%" />
    </div>
    <div class="photo-grid__column">
      <v-img src="https://picsum.photos/500/300?image=22" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=23" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=24" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=25" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=26" style="width:100%" />
      <v-img src="https://picsum.photos/500/300?image=27" style="width:100%" />
    </div>
  </div>
</template>

<style lang="scss">
.photo-grid {
  .container {
    padding: 0;
  }
}
.photo-grid__column {
  -ms-flex: 50%; /* IE10 */
  flex: 50%;
  max-width: 50%;
  padding: 0 4px;
  div {
    margin-top: 4px;
    vertical-align: middle;
  }
}
</style>
