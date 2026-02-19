<script setup>
const steps = [
  {
    title: 'Primo colloquio e obiettivi',
    text: 'Nel primo incontro definiamo insieme la richiesta, il contesto personale e gli obiettivi clinici su cui lavorare.',
  },
  {
    title: 'Percorso e verifiche periodiche',
    text: 'Il percorso viene strutturato in modo personalizzato, con momenti di verifica periodica per valutare andamento, benefici e possibili aggiustamenti.',
  },
  {
    title: 'Durata e frequenza',
    text: 'Durata e frequenza degli incontri vengono concordate in base ai bisogni, con una pianificazione sostenibile e chiara fin dall inizio.',
  },
  {
    title: 'Come capire se e il percorso giusto',
    text: 'La qualita del percorso si misura con indicatori concreti: maggiore consapevolezza, riduzione del disagio e strumenti pratici da usare nella quotidianita.',
  },
]
</script>

<template>
  <section id="come-funziona" class="scroll-mt-20 bg-[#EEE4D7]">
    <div class="mx-auto max-w-6xl px-4 py-16 sm:px-6 lg:px-8 lg:py-20">
      <p class="text-sm font-semibold uppercase tracking-[0.14em] ">Percorso terapeutico</p>
      <h2 class="mt-3 text-3xl font-semibold tracking-tight  sm:text-4xl">Come funziona</h2>

      <div class="mt-10 grid gap-8 lg:grid-cols-5">
        <div class="space-y-4 lg:col-span-3">
          <article
            v-for="(step, index) in steps"
            :key="step.title"
            class="rounded-2xl border border-stone-300 bg-[#F7F1E8] p-6 shadow-sm"
          >
            <div class="flex items-start gap-4">
              <span
                class="inline-flex h-9 w-9 shrink-0 items-center justify-center rounded-full border border-stone-400 bg-[#D6C1A8] text-sm font-semibold"
              >
                {{ index + 1 }}
              </span>
              <div>
                <h3 class="text-xl font-semibold">{{ step.title }}</h3>
                <p class="mt-2 leading-relaxed">{{ step.text }}</p>
              </div>
            </div>
          </article>
        </div>

        <aside class="rounded-3xl border border-stone-300 bg-[#F9F4EE] p-7 shadow-sm lg:col-span-2 lg:p-8">
          <h3 class="text-2xl font-semibold">Dove lavoro e come</h3>
          <p class="mt-4 leading-relaxed">
            Offro prestazioni a domicilio per persone con disabilita, anziani e persone con patologie neurodegenerative.
          </p>
          <p class="mt-4 leading-relaxed">
            In alternativa ricevo in studio a Carrara Avenza, in Via Vico Fiaschi 69/b, presso il centro multidisciplinare
            Aequilibrium Health Center.
          </p>
        </aside>
      </div>
    </div>
  </section>
</template>
