<script setup>
import { ref } from "vue";

const profile = "Ari Wibowo";
const timeline = [
  { year: 1999, event: "Kelahiran di Lampung, Indonesia." },
  {
    year: 1910,
    event: "Menyelesaikan sekolah dasar di MIN 3 Lampung Barat.",
  },
  {
    year: 2014,
    event:
      "Menyelesaikan sekolah menengah Pertama di Madrasah Tsanawiyah Darush sholihin Lampung Barat.",
  },
  {
    year: 2017,
    event:
      "Menyelesaikan sekolah menengah Atas di Madrasah Aliyah Darus sholihin Lampung Barat.",
  },
  {
    year: 2017,
    event: "Admin penjualan | Handala Sweet Ice Cream Depok.",
  },
  {
    year: 2018,
    event:
      "Satuan Pengamanan | PT. Bhawata Nusa Surya Perdana | client(PT. Bank Central Asia).",
  },
  {
    year: 2020,
    event:
      "Satuan Pengamanan | PT. Garda Utama Nasional | client(PT. Bank Central Asia).",
  },
  {
    year: 2024,
    event:
      "Full Stack Web Developer (magang) | CV. Krista Artha Sentosa (fit place).",
  },
  {
    year: 2025,
    event: "Menyelesaikan studi S1 Sistem Informasi di Universitas Terbuka.",
  },
  {
    year: 2025,
    event: "Junior Financial Consultant | Royal Trust Futures.",
  },
];
</script>

<template class="max-w-4xl mx-auto flex flex-col items-center justify-center bg-white shadow-lg overflow-hidden">
  <header
    class="w-full text-center p-10 bg-gradient-to-r from-slate-800 to-gray-700 text-white"
  >
    <h1 class="text-4xl font-extrabold mb-2">{{ profile }}</h1>
    <p class="text-lg font-medium italic">Web Dev</p>
  </header>
  <main class="p-8 space-y-8">
    <figure class="flex flex-col items-center text-center">
      <img
        class="rounded-xl shadow-md mb-4 border"
        width="200"
        src="/images/profile_ariwibowo.webp"
        alt="presiden soekarno"
      />
      <figcaption class="text-sm text-gray-400">
        Oleh -
        <a
          target="_blank"
          class="external text"
          href="https://instagram.com/aariiwiiboowoo"
          >@aariiwiiboowoo
        </a>
      </figcaption>
    </figure>
    <section id="tribute-info">
      <h2 class="text-2xl font-bold text-center mb-6">
        Linimasa kehidupan {{ profile }}
      </h2>
      <ul
        class="space-y-4 border-l-4 border-red-500 pl-6 max-w-2xl mx-auto text-justify"
      >
        <li v-for="item in timeline" :key="item.year">
          <span class="font-bold">{{ item.year }}</span> - {{ item.event }}
        </li>
      </ul>
    </section>
    <footer class="text-center pt-6 border-t mt-6">
      <p class="text-gray-400 text-md font-light">
        Made with ❤️ . by
        <a
          class="hover:underline"
          href="https://ariwibowoedu.github.io/portofolio-v6"
          target="_blank"
        >
          ariwibowoedu.github.io
        </a>
      </p>
    </footer>
  </main>
</template>


