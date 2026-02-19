<script setup>
import { ref } from 'vue'

const isMobileMenuOpen = ref(false)

const menuItems = [
  { label: 'Home', href: '#home' },
  { label: 'A chi mi rivolgo', href: '#a-chi-mi-rivolgo' },
  { label: 'Servizi', href: '#servizi' },
  { label: 'Il mio approccio', href: '#il-mio-approccio' },
  { label: 'Come funziona', href: '#come-funziona' },
  { label: 'Bio', href: '#bio' },
  { label: 'Contatti', href: '#contatti' },
]

function closeMobileMenu() {
  isMobileMenuOpen.value = false
}
</script>

<template>
  <header class="sticky top-0 z-50 border-b border-stone-200 bg-[#F9F4EE]">
    <nav
      class="mx-auto flex max-w-6xl items-center justify-between px-4 py-4 sm:px-6 lg:px-8"
      aria-label="Main navigation"
    >
      <a href="#home" class="inline-flex items-center" aria-label="Home">
        <img src="/LogoGM.png" alt="Logo Giuseppe Marchi" class="h-10 w-auto sm:h-12" />
      </a>

      <ul class="hidden items-center gap-6 md:flex">
        <li v-for="item in menuItems" :key="item.href">
          <a :href="item.href" class="text-sm font-medium text-stone-700 transition hover:text-stone-900">
            {{ item.label }}
          </a>
        </li>
      </ul>

      <button
        class="inline-flex items-center justify-center rounded-md border border-stone-300 px-4 py-2 text-base font-medium text-stone-800 md:hidden"
        type="button"
        :aria-expanded="isMobileMenuOpen"
        aria-controls="mobile-menu"
        @click="isMobileMenuOpen = !isMobileMenuOpen"
      >
        {{ isMobileMenuOpen ? 'Chiudi' : 'Menu' }}
      </button>
    </nav>

    <div
      id="mobile-menu"
      v-show="isMobileMenuOpen"
      class="fixed inset-0 z-40 border-t border-stone-200 bg-[#F9F4EE] pt-24 md:hidden"
    >
      <ul class="flex h-full flex-col gap-3 px-6 py-6">
        <li v-for="item in menuItems" :key="item.href">
          <a
            :href="item.href"
            class="block rounded-xl border border-stone-300 px-4 py-4 text-2xl font-semibold text-stone-700 hover:bg-stone-100 hover:text-stone-900"
            @click="closeMobileMenu"
          >
            {{ item.label }}
          </a>
        </li>
      </ul>
    </div>
  </header>
</template>
