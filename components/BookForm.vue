<template>
  <v-layout
    class="book-form"
    justify-start
    align-center>
    <div>
      <div class="book-form__title">Book your session now</div>
      <v-layout
        justify-start
        align-center>
        <v-layout
          class="book-form__controls"
          fluid
          align-center
          justify-start>
          <div>
            <v-menu
              ref="menu"
              :close-on-content-click="false"
              v-model="menu"
              :nudge-right="40"
              :return-value.sync="date"
              lazy
              transition="scale-transition"
              offset-y
              full-width
              max-width="290px"
              min-width="290px"
            >
              <v-text-field
                slot="activator"
                v-model="date"
                label="Dates"
                readonly
              />
              <v-date-picker
                v-model="date"
                no-title
                scrollable>
                <v-spacer/>
                <v-btn
                  flat
                  color="primary"
                  @click="menu = false">Cancel</v-btn>
                <v-btn
                  flat
                  color="primary"
                  @click="$refs.menu.save(date)">OK</v-btn>
              </v-date-picker>
            </v-menu>
          </div>
          <div class="book-form__control">
            <label>Session</label>
            <v-select
              v-model="session"
              :items="items"/>
          </div>
          <div class="book-form__control">
            <label>Location</label>
            <v-select
              v-model="location"
              :items="locations"/>
          </div>
        </v-layout>
        <div class="book-form__search">
          <v-btn
            icon
            large
            color="white">
            <v-icon>search</v-icon>
          </v-btn>
        </div>
      </v-layout>
    </div>
  </v-layout>
</template>

<script>
export default {
  data: () => ({
    date: new Date().toISOString().substr(0, 10),
    session: 'Morning',
    location: 'Jakarta',
    menu: false,
    items: ['Morning', 'Afternoon', 'Night'],
    locations: ['Jakarta', 'Bogor', 'Depok', 'Tangerang', 'Bekasi']
  })
}
</script>

<style lang="scss">
.book-form {
  padding: 0 100px;
  height: 80%;
}
.book-form__title {
  font-size: 5rem;
  font-weight: bold;
  color: white;
  margin-bottom: 0.5em;
}
.book-form__controls {
  background-color: white;
  padding: 10px 20px;
  border-radius: 4px !important;
  box-shadow: 0px 3px 1px -2px rgba(0, 0, 0, 0.2),
    0px 2px 2px 0px rgba(0, 0, 0, 0.14), 0px 1px 5px 0px rgba(0, 0, 0, 0.12) !important;
  .v-messages {
    display: none;
  }
  .v-text-field__details {
    display: none;
  }
  .v-text-field > .v-input__control > .v-input__slot:before,
  .v-text-field > .v-input__control > .v-input__slot:after {
    display: none;
  }
  .v-input__slot {
    margin-bottom: 0;
  }
  .v-select {
    padding-top: 0;
    margin-top: 0;
  }
  label {
    color: rgba(0, 0, 0, 0.54);
  }
  .v-select__selection--comma {
    margin: 3px 4px 7px 0;
  }
  .v-select__slot {
    max-width: 200px;
  }
}
.book-form__control {
  margin-right: 1em;
}
.book-form__search {
  margin-left: 1em;
}
</style>
