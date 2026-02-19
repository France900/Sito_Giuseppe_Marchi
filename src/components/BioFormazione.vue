<script setup>
const formazione = [
  {
    titolo: 'Laurea in Psicologia Clinica - Universita degli studi di Pisa',
    dettaglio:
      "Tesi triennale sui disturbi del sonno nella malattia di Alzheimer e tesi magistrale sui fattori genetici ed epigenetici del Disturbo da Deficit dell'Attenzione e Iperattivita (ADHD).",
  },
  {
    titolo: 'Master Universitario di II livello in Neuropsicologia Clinica del ciclo di vita - Universita Europea di Roma',
    dettaglio:
      "Percorso completato con una tesi sull'uso di tecniche di stimolazione cognitiva nella malattia di Alzheimer.",
  },
  {
    titolo: 'Neuroscienze Comportamentali - Universita Cattolica del Sacro Cuore (Milano)',
    dettaglio:
      'Attualmente approfondisco prevenzione, diagnosi e intervento in persone con problematiche psichiatriche, neurologiche e neurodegenerative.',
  },
  {
    titolo: 'Laurea Magistrale in Neurobiologia - Universita degli studi di Pavia',
    dettaglio:
      'Percorso in corso per approfondire le basi biologiche del comportamento in condizioni normali e patologiche, con un approccio clinico orientato alla ricerca e in continua evoluzione.',
  },
]
</script>

<template>
  <section id="bio" class="scroll-mt-20 bg-[#F1E7D8]">
    <div class="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-20">
      <div class="flex flex-col gap-4">
        <p class="text-sm font-semibold uppercase tracking-[0.14em]">Profilo professionale</p>
        <h2 class="text-3xl font-semibold tracking-tight sm:text-4xl">Biografia, studi e formazione</h2>
        <p class="max-w-4xl leading-relaxed">
          Mi sono formato in ambito clinico e neuropsicologico con un percorso progressivo tra universita,
          master specialistici e approfondimenti in neuroscienze. L'obiettivo e offrire una pratica clinica solida,
          aggiornata e basata su evidenze, integrando lettura psicologica e conoscenza neurobiologica.
        </p>
      </div>

      <div class="mt-10 flex flex-col gap-5">
        <article
          v-for="item in formazione"
          :key="item.titolo"
          class="rounded-3xl border border-stone-300 bg-[#FAF6F0] p-6 shadow-sm sm:p-8"
        >
          <h3 class="text-xl font-semibold sm:text-2xl">{{ item.titolo }}</h3>
          <p class="mt-3 leading-relaxed">{{ item.dettaglio }}</p>
        </article>
      </div>
    </div>
  </section>
</template>
