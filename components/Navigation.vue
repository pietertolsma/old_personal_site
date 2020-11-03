<template>
  <v-container class="nav-cont">
    <v-row class="nav-row">
      <v-col class="float-left" md="6" sm="6" xs="6">
        <div />
      </v-col>
      <v-col class="right" md="6" sm="6" xs="6">
        <div/>
      </v-col>
    </v-row>
  </v-container>
</template>
<style lang="scss">
.nav-row {
  z-index: 10;
  a {
    text-decoration: none;
    color: white;
    font-size: 1.2em;
  }

  a:hover {
    color: gray;
  }
  .right {
    a {
      margin: 0 10px;
    }
  }
}
</style>
