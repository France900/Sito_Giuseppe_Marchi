<script setup>
const currentYear = new Date().getFullYear()

const quickLinks = [
  { label: 'Home', href: '#home' },
  { label: 'A chi mi rivolgo', href: '#a-chi-mi-rivolgo' },
  { label: 'Servizi', href: '#servizi' },
  { label: 'Il mio approccio', href: '#il-mio-approccio' },
  { label: 'Come funziona', href: '#come-funziona' },
  { label: 'Biografia', href: '#bio' },
]
</script>

<template>
  <footer id="contatti" class="scroll-mt-24 border-t border-stone-200 bg-[#F9F4EE]">
    <div class="mx-auto flex max-w-6xl flex-col gap-10 px-4 py-14 sm:px-6 lg:flex-row lg:items-start lg:gap-12 lg:px-8">
      <section class="lg:flex-[2]">
        <h2 class="text-2xl font-semibold">Giuseppe Marchi</h2>
        <p class="mt-2 text-sm">Psicologo clinico e consulente in neuropsicologia</p>
        <p class="mt-4 max-w-md text-sm leading-relaxed">
          Visite a domicilio e ricevo su appuntamento in studio presso Aequilibrium Health Center in via Vico Fiaschi 69/b, Carrara Avenza.
        </p>
      </section>

      <section class="lg:flex-1">
        <h3 class="text-sm font-semibold uppercase tracking-wide">Contatti</h3>
        <ul class="mt-4 space-y-2 text-sm">
          <li><a class="hover:text-stone-900" href="tel:+393472973026">+39 347 297 3026</a></li>
          <li><a class="hover:text-stone-900" href="mailto:giuseppemarchi94@gmail.com">giuseppemarchi94@gmail.com</a></li>
          <li><a class="hover:text-stone-900" href="mailto:giuseppe.marchi01@universitadipavia.com">giuseppe.marchi01@universitadipavia.com</a></li>
          <li>via Vico Fiaschi 69/b</li>
          <li>Lun - Ven: 9:00 - 19:00</li>
        </ul>
      </section>

      <section class="lg:flex-1">
        <h3 class="text-sm font-semibold uppercase tracking-wide">Link rapidi</h3>
        <ul class="mt-4 space-y-2 text-sm">
          <li v-for="item in quickLinks" :key="item.href">
            <a :href="item.href" class="hover:text-stone-900">{{ item.label }}</a>
          </li>
        </ul>
      </section>
    </div>

    <div class="border-t border-stone-200">
      <div class="mx-auto flex max-w-6xl flex-col gap-3 px-4 py-5 text-xs sm:px-6 lg:flex-row lg:items-center lg:justify-between lg:px-8">
        <p>� {{ currentYear }} Giuseppe Marchi p.iva: 02750670461</p>
        <p class="flex flex-wrap gap-4">
          Iscrizione alla sezione A dell’albo degli Psicologi della Toscana n.11327
        </p>
      </div>
    </div>
  </footer>
</template>
