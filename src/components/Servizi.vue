<script setup>
const services = [
  'Colloquio individuale',
  'Sostegno ai familiari',
  'Orientamento e collaborazione con rete di cura',
]
</script>

<template>
  <section id="servizi" class="scroll-mt-20 bg-[#B5A085]">
    <div class="mx-auto flex max-w-6xl flex-col gap-10 px-4 py-16 sm:px-6 lg:flex-row lg:items-center lg:px-8 lg:py-20">
      <div class="flex-1">
        <h2 class="text-3xl font-semibold tracking-tight sm:text-4xl">Servizi</h2>
        <ul class="mt-8 space-y-4">
          <li
            v-for="service in services"
            :key="service"
            class="rounded-2xl border border-stone-300 bg-[#F4EEE5] px-6 py-5 text-lg font-medium shadow-sm"
          >
            {{ service }}
          </li>
        </ul>
      </div>

      <div class="flex flex-1 justify-center lg:justify-end">
        <img
          src="/frattale.png"
          alt="Frattale asimmetrico arboreo"
          class="w-full max-w-md rounded-3xl"
        />
      </div>
    </div>
  </section>
</template>
