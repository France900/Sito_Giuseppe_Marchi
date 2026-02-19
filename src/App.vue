<script setup>
import Home from './components/Home.vue'
import Navbar from './components/Navbar.vue'
import AChiMiRivolgo from './components/AChiMiRivolgo.vue'
import Servizi from './components/Servizi.vue'
import IlMioApproccio from './components/IlMioApproccio.vue'
import ComeFunziona from './components/ComeFunziona.vue'
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

      <section id="bio" class="scroll-mt-24 mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-24">
      </section>
    </main>

    <Footer />
  </div>
</template>
