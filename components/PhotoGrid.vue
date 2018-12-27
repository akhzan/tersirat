<template>
  <!-- <v-layout class="photo-grid">
    <v-flex xs12 sm12 md12>
      <div>
        <v-container grid-list-sm fluid>
          <v-layout row wrap>
            <v-flex v-for="n in 9" :key="n">
              <v-card flat tile class="d-flex">
                <v-img
                  :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                  :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
                  height="250"
                  width="250"
                  class="grey lighten-2"
                >
                  <v-layout slot="placeholder" fill-height align-center justify-center ma-0>
                    <v-progress-circular indeterminate color="grey lighten-5"/>
                  </v-layout>
                </v-img>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </div>
    </v-flex>
  </v-layout> -->
  <div class="photo-grid__row">
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
.photo-grid__row {
  display: -ms-flexbox; /* IE10 */
  display: flex;
  -ms-flex-wrap: wrap; /* IE10 */
  flex-wrap: wrap;
  margin: 0 -4px;
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
