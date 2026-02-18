<script setup>
const cards = [
  {
    title: 'Sviluppo',
    text: `Offro consulenza e interventi nell'ambito delle problematiche legate al Neurosviluppo, come l'ADHD e i disturbi dell'apprendimento nell'ambito scolastico.`,
  },
  {
    title: 'Adulti',
    text: `Offro consulenza e interventi psicoeducativi per adulti, in particolare disturbi alimentari, ADHD nell'adulto, e interventi in pazienti con patologie organiche (ad es.: traumi cerebrali, ischemie)`,
  },
  {
    title: 'Anziani e caregivers',
    text: `Consulenza, supporto riabilitazione/stimolazione cognitiva in pazienti anziani, con disabilita e/o con patologie neurodegenerative. Supporto e formazione ai familiari di pazienti con patologie neurodegenerative (ad es.: alzheimer)`,
  },
]
</script>

<template>
  <section id="a-chi-mi-rivolgo" class="scroll-mt-20 mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-20">
    <h2 class="text-3xl font-semibold tracking-tight sm:text-4xl">A chi mi rivolgo</h2>

    <div class="mt-10 grid gap-6 md:grid-cols-3 xl:grid-cols-3">
      <article
        v-for="card in cards"
        :key="card.title"
        class="rounded-2xl border border-stone-300 bg-[#F4EEE5] p-6 shadow-sm"
      >
        <h3 class="text-2xl font-semibold">{{ card.title }}</h3>
        <p class="mt-4 leading-relaxed">{{ card.text }}</p>
      </article>
    </div>
  </section>
</template>
