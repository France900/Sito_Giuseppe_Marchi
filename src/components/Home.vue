<script setup>
const whatsappNumber = '+39 347 297 3026'
</script>

<template>
  <section id="home" class="bg-[#D6D4C8] text-[#66635A]">
    <div class="mx-auto grid max-w-6xl gap-10 px-4 py-16 sm:px-6 lg:grid-cols-2 lg:items-center lg:px-8 lg:py-24">
      <div class="order-1">
        <h1 class="text-4xl font-semibold tracking-tight sm:text-5xl">Giuseppe Marchi</h1>
        <p class="mt-1 ml-4 text-lg sm:text-xl">Psicologo a indirizzo clinico</p>
        <p class="mt-1 ml-6 text-lg sm:text-xl">Esperto in neuropsicologia clinica</p>
        <a
          :href="`https://wa.me/${whatsappNumber}`"
          target="_blank"
          rel="noopener noreferrer"
          class="mt-8 ml-16 inline-flex flex-col rounded-xl border border-[#66635A] px-5 py-3 text-left transition hover:bg-[#66635A] hover:text-[#D6D4C8]"
        >
          <span class="text-sm font-medium">Per ulteriori informazioni scrivimi su WhatsApp </span>
          <span class="mt-1 text-base font-semibold">{{ whatsappNumber }}</span>
        </a>
      </div>

      <div class="order-2 flex justify-center lg:justify-end">
        <img
          src="/imgHero.png"
          alt="Giuseppe Marchi"
          class="w-full object-cover"
        />
      </div>
    </div>
  </section>
</template>
