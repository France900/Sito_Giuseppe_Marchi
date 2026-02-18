<script setup>
import Home from './components/Home.vue'
import Navbar from './components/Navbar.vue'
</script>

<template>
  <div class="min-h-screen bg-[#F9F4EE] text-stone-900">
    <Navbar />

    <main>
      <Home />

      <section id="a-chi-mi-rivolgo" class="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-24">
      </section>

      <section id="servizi" class="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-24">
      </section>

      <section id="come-funziona" class="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-24">
      </section>

      <section id="bio" class="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-24">
      </section>
    </main>

    <footer id="contatti" class="border-t border-stone-200 bg-[#F9F4EE]">
      <div class="mx-auto max-w-6xl px-4 py-14 sm:px-6 lg:px-8"></div>
    </footer>
  </div>
</template>
