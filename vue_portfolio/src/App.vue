<template>
    <div>
      <Navbar />
      <Hero />
      <Skills />
      <Portfolio />
      <Contact />
      <Footer />
    </div>
</template>

<script>
import Navbar from './components/Navbar'
import Hero from './components/Hero'
import Skills from './components/Skills'
import Portfolio from './components/Portfolio'
import Contact from './components/Contact'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    Skills,
    Portfolio,
    Contact,
    Footer
  },
}
</script>

<style>

</style>
