<template>
  <Navbar />
  <!-- <Home />
  <AppFooter /> -->
  <router-view/>
</template>


<script>

import Navbar from './components/Navbar'
import Home from './views/Home'
import AppFooter from './components/AppFooter'

export default {
  
  components: { Navbar, Home, AppFooter }

}
</script>