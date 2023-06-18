<script setup>
import GraficoDona from "./components/GraficoDona.vue";
import GraficoBarra from "./components/GraficoBarra.vue";
import GraficoDona2 from "./components/GraficoDona2.vue";
import GraficoLinea from "./components/GraficoLinea.vue";
import GraficoLinea2 from "./components/GraficoLinea2.vue";
import GraficoProgreso from "./components/GraficoProgreso.vue";
import Slider from "./components/Slider.vue";
import Navbar from "./components/Navbar.vue";
import Breadcrumb from "./components/Breadcrumb.vue";
</script>

<template>
  <Navbar />
  <Breadcrumb />
  <div class="flex h-screen">
    <div
      class="grid w-1/2 grid-cols-2 grid-rows-5 items-center gap-4 bg-fondo p-2"
    >
      <div class="col-span-2 flex h-full justify-center rounded-lg bg-gray-700">
        <GraficoDona2 class="w-1/2 p-2" /> <GraficoBarra class="w-50" />
      </div>

      <div class="row-start-2 h-full rounded-lg bg-gray-700">
        <GraficoProgreso />
      </div>

      <div class="row-start-2 h-full rounded-lg bg-gray-700">
        <GraficoLinea2 />
      </div>

      <div class="flex h-full justify-center rounded-lg bg-gray-700">
        <GraficoDona />
      </div>

      <div class="row-start-3 h-full rounded-lg bg-gray-700">
        <GraficoLinea />
      </div>
    </div>

    <div class="w-1/2 flex-col bg-fondo p-2">
      <div
        class="flex h-56 justify-center rounded-xl bg-gradient-to-r from-teal-400 to-teal-700"
      >
        <GraficoBarra />
      </div>
      <div class="mt-2 rounded-xl">
        <h1 class="mb-2 text-xl font-semibold text-white">Event Galleries</h1>
        <Slider />
      </div>
    </div>
  </div>
</template>

<style></style>
