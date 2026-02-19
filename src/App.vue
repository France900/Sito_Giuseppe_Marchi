<script setup>
import Home from './components/Home.vue'
import Navbar from './components/Navbar.vue'
import AChiMiRivolgo from './components/AChiMiRivolgo.vue'
import Servizi from './components/Servizi.vue'
import IlMioApproccio from './components/IlMioApproccio.vue'
import ComeFunziona from './components/ComeFunziona.vue'
import BioFormazione from './components/BioFormazione.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <div id="home">
    <Navbar />

    <main>
      <Home />
      <AChiMiRivolgo />
      <Servizi />
      <IlMioApproccio />
      <ComeFunziona />
      <BioFormazione />
    </main>

    <Footer />
  </div>
</template>
