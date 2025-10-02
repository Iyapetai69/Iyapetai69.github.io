+++
title = "Prediksi Togel Hari Ini"
description = "Update angka main, paito, syair, dan prediksi harian."
+++

<!-- Section Welcome -->
<section class="bg-pink-100 rounded-2xl shadow-md p-6 mb-8 text-center">
  <h1 class="text-3xl font-bold text-pink-700 mb-2">Selamat Datang!</h1>
  <p class="text-gray-700">
    Situs ini menyediakan prediksi angka harian, live draw, paito, dan syair dari 5 pasaran utama.  
    <br>Disclaimer: Prediksi hanya hiburan semata.
  </p>
</section>

<!-- Section Pasaran -->
<section class="mb-12">
  <h2 class="text-2xl font-semibold text-pink-600 mb-6 text-center">Pasaran Utama</h2>
  <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-6">
    <!-- Singapore -->
    <div class="bg-white rounded-xl shadow hover:shadow-lg p-4 text-center">
      <img src="/images/sgp.png" alt="Singapore" class="mx-auto mb-3 rounded-lg">
      <h3 class="text-lg font-bold text-pink-700">Singapore</h3>
      <div class="mt-2 flex flex-col gap-2">
        <a href="/singapore/" class="bg-pink-500 text-white py-1 px-3 rounded-lg hover:bg-pink-600">Prediksi</a>
        <a href="/live-draw/" class="text-pink-600 hover:underline">Live Draw</a>
        <a href="/paito/" class="text-pink-600 hover:underline">Paito</a>
        <a href="/syair/" class="text-pink-600 hover:underline">Syair</a>
      </div>
    </div>

    <!-- Hongkong -->
    <div class="bg-white rounded-xl shadow hover:shadow-lg p-4 text-center">
      <img src="/images/hk.png" alt="Hongkong" class="mx-auto mb-3 rounded-lg">
      <h3 class="text-lg font-bold text-pink-700">Hongkong</h3>
      <div class="mt-2 flex flex-col gap-2">
        <a href="/hongkong/" class="bg-pink-500 text-white py-1 px-3 rounded-lg hover:bg-pink-600">Prediksi</a>
        <a href="/live-draw/" class="text-pink-600 hover:underline">Live Draw</a>
        <a href="/paito/" class="text-pink-600 hover:underline">Paito</a>
        <a href="/syair/" class="text-pink-600 hover:underline">Syair</a>
      </div>
    </div>

    <!-- Sydney -->
    <div class="bg-white rounded-xl shadow hover:shadow-lg p-4 text-center">
      <img src="/images/sydney.png" alt="Sydney" class="mx-auto mb-3 rounded-lg">
      <h3 class="text-lg font-bold text-pink-700">Sydney</h3>
      <div class="mt-2 flex flex-col gap-2">
        <a href="/sydney/" class="bg-pink-500 text-white py-1 px-3 rounded-lg hover:bg-pink-600">Prediksi</a>
        <a href="/live-draw/" class="text-pink-600 hover:underline">Live Draw</a>
        <a href="/paito/" class="text-pink-600 hover:underline">Paito</a>
        <a href="/syair/" class="text-pink-600 hover:underline">Syair</a>
      </div>
    </div>

    <!-- Japan -->
    <div class="bg-white rounded-xl shadow hover:shadow-lg p-4 text-center">
      <img src="/images/japan.png" alt="Japan" class="mx-auto mb-3 rounded-lg">
      <h3 class="text-lg font-bold text-pink-700">Japan</h3>
      <div class="mt-2 flex flex-col gap-2">
        <a href="/japan/" class="bg-pink-500 text-white py-1 px-3 rounded-lg hover:bg-pink-600">Prediksi</a>
        <a href="/live-draw/" class="text-pink-600 hover:underline">Live Draw</a>
        <a href="/paito/" class="text-pink-600 hover:underline">Paito</a>
        <a href="/syair/" class="text-pink-600 hover:underline">Syair</a>
      </div>
    </div>

    <!-- Taiwan -->
    <div class="bg-white rounded-xl shadow hover:shadow-lg p-4 text-center">
      <img src="/images/taiwan.png" alt="Taiwan" class="mx-auto mb-3 rounded-lg">
      <h3 class="text-lg font-bold text-pink-700">Taiwan</h3>
      <div class="mt-2 flex flex-col gap-2">
        <a href="/taiwan/" class="bg-pink-500 text-white py-1 px-3 rounded-lg hover:bg-pink-600">Prediksi</a>
        <a href="/live-draw/" class="text-pink-600 hover:underline">Live Draw</a>
        <a href="/paito/" class="text-pink-600 hover:underline">Paito</a>
        <a href="/syair/" class="text-pink-600 hover:underline">Syair</a>
      </div>
    </div>
  </div>
</section>

<!-- Section Prediksi -->
<section class="bg-pink-50 rounded-2xl shadow-md p-6">
  <h2 class="text-2xl font-semibold text-pink-600 mb-6 text-center">Prediksi Terbaru</h2>
  <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-4">
    {{ range first 5 (where .Site.RegularPages "Section" "singapore") }}
    <article class="bg-white rounded-lg p-3 shadow hover:shadow-lg">
      <a href="{{ .RelPermalink }}" class="text-pink-700 font-bold hover:underline">
        {{ .Title }}
      </a>
      <p class="text-gray-500 text-sm">{{ .Date.Format "02 Jan 2006" }}</p>
    </article>
    {{ end }}
  </div>
</section>
