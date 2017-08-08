<template>
  <div>
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

