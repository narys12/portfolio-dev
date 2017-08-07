<template>
  <div>
    <v-toolbar flat>
      <v-spacer></v-spacer>
      <v-toolbar-side-icon class="hidden-md-and-up"></v-toolbar-side-icon>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat>Home</v-btn>
        <v-btn flat>About</v-btn>
        <v-btn flat>Web Crawling</v-btn>
        <v-btn flat>Web Development</v-btn>
        <v-btn flat>Contact</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <Home/>
    <About/>
    <Crawl/>
    <Dev/>
    <Contact/>
  </div>
</template>

<script>
  import Home from '~/components/Home'
  import About from '~/components/About'
  import Crawl from '~/components/Crawl'
  import Dev from '~/components/Dev'
  import Contact from '~/components/Contact'

  export default {
    components: {
      Home,
      Crawl,
      Dev,
      Contact
    }
  }
</script>