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

  <div class="m-4 grid grid-cols-1 gap-4 sm:grid-cols-4">
    <div
      class="h-72 flex-col rounded-lg bg-gray-700 sm:col-span-2 sm:row-span-2"
    >
      <div class="m-4 flex text-white">
        <p>Best selling</p>
        <p class="ml-auto text-gray-500">This week</p>
      </div>
      <div class="m-3 mx-6 flex rounded-lg bg-tarjetas p-1 px-3 text-white">
        <p>Tuesday</p>
        <p class="ml-auto">215.523 pcs</p>
      </div>
      <div class="flex items-center justify-center">
        <div class="w-52 p-2">
          <GraficoDona2 />
        </div>
        <div class="hidden w-64 md:block">
          <GraficoBarra />
        </div>
      </div>
    </div>

    <div class="h-36 rounded-lg bg-gray-700 sm:col-start-1 sm:row-start-3">
      <GraficoProgreso />
    </div>
    <div
      class="flex h-36 justify-center rounded-lg bg-gray-700 sm:col-start-2 sm:row-start-3"
    >
      <GraficoLinea2 />
    </div>
    <div
      class="flex h-36 justify-center rounded-lg bg-gray-700 sm:col-start-1 sm:row-start-4"
    >
      <GraficoDona />
    </div>
    <div
      class="flex h-36 justify-center rounded-lg bg-gray-700 sm:col-start-2 sm:row-start-4"
    >
      <GraficoLinea />
    </div>
    <div
      class="flex h-52 justify-center rounded-lg bg-gradient-to-r from-teal-400 to-teal-700 sm:col-span-2 sm:col-start-3 sm:row-start-1"
    >
      <GraficoBarra />
    </div>
    <div
      class="h-36 rounded-lg sm:col-span-2 sm:col-start-3 sm:row-span-3 sm:row-start-2"
    >
      <h1 class="mb-2 text-xl font-semibold text-white">Event Galleries</h1>
      <Slider class="mb-4" />
    </div>
  </div>
</template>

<style>
.grafico-container {
  max-width: 150px;
}
</style>
