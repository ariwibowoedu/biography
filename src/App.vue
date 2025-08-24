<script setup>
const timeline = [
  { year: 1901, event: "Kelahiran di Surabaya, Indonesia" },
  {
    year: 1915,
    event: "Menyelesaikan sekolah dasar di Europeesche Lagere School (ELS)",
  },
  {
    year: 1921,
    event:
      "Menyelesaikan sekolah menengah Belanda di Hogere Burger School (HBS)",
  },
  {
    year: 1926,
    event:
      "Lulus teknik sipil di Technische Hoogeshchool te Bandoeng (sekarang ITB)",
  },
  { year: 1927, event: "Mendirikan Partai Nasional Indonesia (PNI)" },
  { year: 1929, event: "Ditangkap dan dipenjara di Sukamiskin Bandung" },
  {
    year: 1930,
    event: "Membacakan pidato 'Indonesia Menggugat' di Landraad Bandung",
  },
  { year: 1933, event: "Dibuang ke Ende, Flores" },
  { year: 1942, event: "Bebas dari pengasingan, aktif di BPUPKI" },
  { year: 1945, event: "Dilantik sebagai Presiden pertama Republik Indonesia" },
  { year: 1967, event: "Menjadi tahanan rumah di Bogor" },
  { year: 1970, event: "Wafat di Jakarta" },
];
</script>

<template class="max-w-4xl mx-auto flex flex-col items-center justify-center bg-white shadow-lg overflow-hidden">
  <header
    class="w-full text-center p-10 bg-gradient-to-r from-red-600 to-red-400 text-white"
  >
    <h1 class="text-4xl font-extrabold mb-2">Ir. Soekarno</h1>
    <p class="text-lg font-medium italic">Presiden pertama Indonesia</p>
  </header>
  <main class="p-8 space-y-8">
    <figure class="flex flex-col items-center text-center">
      <img
        class="rounded-xl shadow-md mb-4 border"
        width="200"
        src="/images/Presiden_Sukarno.webp"
        alt="presiden soekarno"
      />
      <figcaption class="text-sm text-gray-400">
        Oleh Onbekend/Anonymous -
        <a
          rel="nofollow"
          class="external text"
          href="http://hdl.handle.net/1887.1/item:782159"
          >KITLV 2691</a
        >, Domain Publik,
        <a href="https://commons.wikimedia.org/w/index.php?curid=9780791"
          >Pranala</a
        >
      </figcaption>
    </figure>
    <section id="tribute-info">
      <h2 class="text-2xl font-bold text-center mb-6">
        Linimasa kehidupan Ir. Soekarno
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
      <p class="text-gray-600">
        Baca lebih lengkap kisahnya di
        <a
          href="https://id.wikipedia.org/wiki/Soekarno"
          target="_blank"
          class="text-blue-500 font-semibold underline"
        >
          wikipedia</a
        >
      </p>
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


