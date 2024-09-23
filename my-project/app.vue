<template>
  <div class="bg-gray-100">
    <header class="fixed top-0 left-0 w-full bg-gray-900 text-white py-4 shadow-lg">
      <div class="container mx-auto flex justify-between items-center">
        <h1 class="text-3xl font-bold transition-transform transform hover:scale-105 ml-5">Portofolio Saya</h1>
        <nav>
          <!-- Add navigation items here if needed -->
        </nav>
      </div>
    </header>

    <main class="container mx-auto px-4 pt-16">
      <nuxt />

      <section class="py-8">
        <div class="bg-gray-100">
          <h2 class="text-3xl font-bold mb-4 ml-9">Tentang Saya</h2>
          <div class="flex flex-col md:flex-row items-center ml-8">
            <img src="assets/img/foto-profil.jpg" alt="Foto Profil" class="w-32 h-34 md:mr-8 rounded-full shadow-md ml-9">
            <div class="ml-8">
  <p class="text-lg mb-2">Nama: Dimas Aminudin Mayoni</p>
  <p class="text-lg mb-2">Umur: 19 Tahun</p>
  <p class="text-lg mb-2">Status: Mahasiswa</p>
  <p class="text-lg">Tentang: Saya adalah seorang mahasiswa yang sedang belajar menjadi web developer yang passionate dengan teknologi web.</p>
</div>
          </div>
        </div>

        <h2 class="text-3xl font-bold mb-4 ml-10 mt-10">My Pictures</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
          <div class="p-4 bg-white rounded-lg shadow-md transition-transform transform hover:scale-105">
            <img src="assets/img/foto1.jpg" alt="Project 1 Image" class="w-full object-cover rounded-lg mb-4">
            <h3 class="text-xl font-bold mb-2">Pictures 1 Title</h3>
            <p>Brief description of Picture 1.</p>
          </div>

          <div class="p-4 bg-white rounded-lg shadow-md transition-transform transform hover:scale-105">
            <img src="assets/img/foto2.jpg" alt="Project 1 Image" class="w-full object-cover rounded-lg mb-4">
            <h3 class="text-xl font-bold mb-2">Pictures 2 Title</h3>
            <p>Brief description of Picture 2.</p>
          </div>

          <div class="p-4 bg-white rounded-lg shadow-md transition-transform transform hover:scale-105">
            <img src="assets/img/foto3.jpg" alt="Project 1 Image" class="w-full object-cover rounded-lg mb-4">
            <h3 class="text-xl font-bold mb-2">Pictures 3 Title</h3>
            <p>Brief description of Picture 3.</p>
          </div>

          
        </div>
      </section>
    </main>
    <br><br><br>
    <footer class="fixed bottom-0 left-0 w-full bg-gray-900 text-white py-4">
      <div class="container mx-auto text-center">
        <p>&copy; {{ new Date().getFullYear() }} Dimas Aminudin Mayoni</p>
      </div>
    </footer>
  </div>
</template>

<style scoped>
  /* Add smooth transition effects */
  .transition-transform {
    transition: transform 0.3s ease;
  }

  .hover\:scale-105:hover {
    transform: scale(1.05);
  }

  /* Adjust footer position for better mobile view */
  @media (max-width: 768px) {
    footer {
      position: relative;
      bottom: auto;
    }
  }
</style>