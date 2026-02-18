<script setup>
const whatsappNumber = '393000000000'
const whatsappDisplay = '+39 300 000 0000'
const whatsappMessage = encodeURIComponent('Ciao Giuseppe, vorrei maggiori informazioni.')
</script>

<template>
  <section id="home" class="bg-[#D6D4C8] text-[#66635A]">
    <div class="mx-auto max-w-7xl px-4 py-10 sm:px-6 lg:px-8 lg:py-14">
      <div class="grid gap-8 lg:grid-cols-12 lg:items-center">
        <div class="relative z-10 lg:col-span-5">
          <h1 class="text-4xl font-semibold leading-tight tracking-tight sm:text-5xl">Giuseppe Marchi</h1>
          <p class="mt-6 text-lg leading-relaxed sm:text-xl">psicologo a indirizzo clinico</p>
          <p class="mt-2 text-lg leading-relaxed sm:text-xl">Esperto in neuropsicologia clinica</p>

          <a
            :href="`https://wa.me/${whatsappNumber}?text=${whatsappMessage}`"
            target="_blank"
            rel="noopener noreferrer"
            class="group mt-9 block w-fit rounded-2xl border border-[#B8B2A7] bg-[#F9F4EE] p-1 shadow-[0_12px_32px_-18px_rgba(66,62,55,0.45)] transition hover:-translate-y-0.5 hover:shadow-[0_20px_34px_-18px_rgba(66,62,55,0.55)]"
          >
            <span class="flex items-center gap-3 rounded-xl bg-white/70 px-5 py-4">
              <span class="inline-block h-2.5 w-2.5 rounded-full bg-[#31C860]"></span>
              <span class="flex flex-col">
                <span class="text-sm font-medium leading-snug text-[#66635A]">
                  Scrivimi su WhatsApp per ulteriori informazioni
                </span>
                <span class="mt-1 text-base font-semibold text-[#4F4B43]">
                  {{ whatsappDisplay }}
                </span>
              </span>
            </span>
          </a>
        </div>

        <div class="lg:col-span-7">
          <div class="relative overflow-hidden rounded-3xl rounded-tl-[180px] bg-[#CFCBBF]">
            <img
              src="/imgHero.png"
              alt="Giuseppe Marchi"
              class="h-[460px] w-full object-cover object-center sm:h-[540px] lg:h-[620px]"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
