<template>
  <v-layout class="app-header" row justify-space-between align-center align-content-center>
    <v-flex>
      <div class="app-header__logo">tersirat</div>
    </v-flex>
    <div class="app-header__right">
      <ul>
        <li><i class="fab fa-instagram" /></li>
        <li><i class="fab fa-whatsapp" /></li>
      </ul>
    </div>
  </v-layout>
</template>

<style lang="scss">
.app-header {
  padding: 40px 40px 0 40px;
  font-size: 1.2rem;
  color: white;
}
.app-header__logo {
  font-size: 1.8rem;
}
.app-header__right {
  padding-right: 1em;
  ul {
    list-style-type: none;
    li {
      display: inline;
      margin-right: 0.75em;
    }
  }
  a {
    color: white;
  }
  i {
    font-size: 1.4rem;
    cursor: pointer;
  }
}
</style>
