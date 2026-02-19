<script setup>
const approachAreas = [
  {
    title: 'Approccio clinico-psicologico',
    text: `Mi occupo di consulenza, valutazione, diagnosi e intervento nell'ambito delle principali problematiche psicologiche, per fornire ai clienti supporto e strumenti per gestire condizioni di disagio come i disturbi d'ansia e dell'umore, disturbi alimentari, disturbi da uso e abuso di sostanze.`,
  },
  {
    title: 'Approccio neuropsicologico',
    text: `La neuropsicologia e' la branca della psicologia che studia le basi anatomiche e fisiologiche dei processi cognitivi, emotivi e comportamentali, in condizioni di normalita' e patologia. Per fare questo si avvale di strumenti come il colloquio, la somministrazione di test psicometrici e l'ausilio fornito da indagini strumentali come TAC o risonanza magnetica. Puo' inoltre prevedere interventi di riabilitazione delle funzioni compromesse da patologie di varia natura, comprese condizioni degenerative, a base genetica o ereditaria, e conseguenti a lesioni, traumi o infezioni del sistema nervoso.`,
  },
]
</script>

<template>
  <section id="il-mio-approccio" class="scroll-mt-20 bg-[#F4EEE5]">
    <div class="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-20">
      <p class="text-sm font-semibold uppercase tracking-[0.14em]">Metodo di lavoro</p>
      <h2 class="mt-3 text-3xl font-semibold tracking-tight sm:text-4xl">Il mio approccio</h2>
      <p class="mt-4 max-w-3xl text-base leading-relaxed sm:text-lg">
        Un percorso costruito su ascolto clinico, strumenti validati e obiettivi concreti, con attenzione alla persona e al suo contesto di vita.
      </p>

      <div class="mt-10 grid gap-6 lg:grid-cols-2">
        <article
          v-for="area in approachAreas"
          :key="area.title"
          class="rounded-3xl border border-stone-300/80 bg-[#FAF6F0] p-7 shadow-sm sm:p-8"
        >
          <h3 class="text-2xl font-semibold">{{ area.title }}</h3>
          <p class="mt-5 leading-relaxed">{{ area.text }}</p>
        </article>
      </div>
    </div>
  </section>
</template>
