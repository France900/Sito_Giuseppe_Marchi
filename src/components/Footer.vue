<script setup>
const currentYear = new Date().getFullYear()

const quickLinks = [
  { label: 'Home', href: '#home' },
  { label: 'A chi mi rivolgo', href: '#a-chi-mi-rivolgo' },
  { label: 'Servizi', href: '#servizi' },
  { label: 'Il mio approccio', href: '#il-mio-approccio' },
  { label: 'Come funziona', href: '#come-funziona' },
  { label: 'Bio', href: '#bio' },
]

const legalLinks = [
  { label: 'Privacy Policy', href: '#' },
  { label: 'Cookie Policy', href: '#' },
  { label: 'Termini e condizioni', href: '#' },
]
</script>

<template>
  <footer id="contatti" class="scroll-mt-24 border-t border-stone-200 bg-[#F9F4EE]">
    <div class="mx-auto grid max-w-6xl gap-10 px-4 py-14 sm:px-6 lg:grid-cols-4 lg:gap-12 lg:px-8">
      <section class="lg:col-span-2">
        <h2 class="text-2xl font-semibold">Giuseppe Marchi</h2>
        <p class="mt-2 text-sm">Psicologo clinico e consulente in neuropsicologia</p>
        <p class="mt-4 max-w-md text-sm leading-relaxed">
          Ricevo su appuntamento in studio e online. Questo footer contiene dati dimostrativi da sostituire con i riferimenti definitivi.
        </p>
      </section>

      <section>
        <h3 class="text-sm font-semibold uppercase tracking-wide">Contatti</h3>
        <ul class="mt-4 space-y-2 text-sm">
          <li><a class="hover:text-stone-900" href="tel:+390212345678">+39 02 1234 5678</a></li>
          <li><a class="hover:text-stone-900" href="mailto:info@giuseppemarchi.it">info@giuseppemarchi.it</a></li>
          <li>Via Esempio 123, Milano (MI)</li>
          <li>Lun - Ven: 9:00 - 19:00</li>
        </ul>
      </section>

      <section>
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
        <p>� {{ currentYear }} Giuseppe Marchi. Tutti i diritti riservati.</p>
        <div class="flex flex-wrap gap-4">
          <a
            v-for="item in legalLinks"
            :key="item.label"
            :href="item.href"
            class="hover:text-stone-900"
          >
            {{ item.label }}
          </a>
          <a href="#" class="hover:text-stone-900">Instagram</a>
          <a href="#" class="hover:text-stone-900">LinkedIn</a>
        </div>
      </div>
    </div>
  </footer>
</template>
