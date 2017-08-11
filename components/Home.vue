<template>
<div id="wrap-banner">
  <v-toolbar dark flat class="transparent" fixed>
    <v-spacer></v-spacer>
    <v-toolbar-side-icon class="hidden-md-and-up" @click.native.stop="drawer = !drawer"></v-toolbar-side-icon>
    <v-toolbar-items class="hidden-sm-and-down menu-items">
      <v-btn flat>Home</v-btn>
      <v-btn flat>About</v-btn>
      <v-btn flat>Web Crawling</v-btn>
      <v-btn flat>Web Development</v-btn>
      <v-btn flat>Contact</v-btn>
    </v-toolbar-items>
  </v-toolbar>
  <v-navigation-drawer class="pb-0" persistent absolute height="100%" dark enable-resize-watcher temporary v-model="drawer">
    <v-list dense>
      <v-subheader class="mt-3 grey--text text--darken-1">MEGA BANG</v-subheader>
      <v-list-tile class="mt-3">
        <v-list-tile-action>
          <v-icon class="grey--text text--darken-1">home</v-icon>
        </v-list-tile-action>
        <v-list-tile-title class="grey--text text--darken-1">Home</v-list-tile-title>
      </v-list-tile>
      <v-list-tile>
        <v-list-tile-action>
          <v-icon class="grey--text text--darken-1">info</v-icon>
        </v-list-tile-action>
        <v-list-tile-title class="grey--text text--darken-1">About</v-list-tile-title>
      </v-list-tile>
      <v-list-tile>
        <v-list-tile-action>
          <v-icon class="grey--text text--darken-1">web</v-icon>
        </v-list-tile-action>
        <v-list-tile-title class="grey--text text--darken-1">Web Crawling</v-list-tile-title>
      </v-list-tile>
      <v-list-tile>
        <v-list-tile-action>
          <v-icon class="grey--text text--darken-1">code</v-icon>
        </v-list-tile-action>
        <v-list-tile-title class="grey--text text--darken-1">Web Development</v-list-tile-title>
      </v-list-tile>
      <v-list-tile>
        <v-list-tile-action>
          <v-icon class="grey--text text--darken-1">contact_mail</v-icon>
        </v-list-tile-action>
        <v-list-tile-title class="grey--text text--darken-1">Contact</v-list-tile-title>
      </v-list-tile>
    </v-list>
  </v-navigation-drawer>
  <div class="main-section">
    <div class="title">
      <h2>Mega Bang</h2>
      <h4>The birth of a dream</h4>
    </div>
  </div>
  <div class="next mb-3">
    <v-btn icon dark class="transparent btn-next">
      <v-icon large>arrow_downward</v-icon>
    </v-btn>
  </div>

  <vue-particles color="#dedede" :particleOpacity="1" :particlesNumber="80" shapeType="circle" :particleSize="4" linesColor="#dedede" :linesWidth="1" :lineLinked="true" :lineOpacity="0.4" :linesDistance="150" :moveSpeed="3" :hoverEffect="true" hoverMode="grab"
    :clickEffect="true" clickMode="push">
  </vue-particles>
</div>
</template>

<script>
  export default {
    data: () => ({
      drawer: false
    })
  }
</script>

<style lang="css" scoped>
    #wrap-banner {
        text-align: center;
    }

    #particles-js {
        background-color: black;
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }

    .main-section {
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        -webkit-align-items: center;
        -ms-flex-align: center;
        align-items: center;
        display: -webkit-flex;
        display: flex;
        justify-content: center;
    }

    .title {
        z-index: 99;
    }

    h2,
    h4 {
        margin: 0;
    }

    .next {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
    }

    .btn-next {
        z-index: 1;
    }
</style>
