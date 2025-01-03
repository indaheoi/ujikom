<template>
  <!-- component -->
  <div class="bg">
    <section class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-4 py-12">
      <div class="text-center pb-12">
        <h1 class="font-bold text-3xl md:text-4xl lg:text-5xl font-heading text-gray-900">Galeri SMKN 4 Tasikmalaya</h1>
      </div>

      <!-- Galeri Grid -->
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Render galeri secara dinamis -->
        <div v-for="(item, index) in visibleItems" :key="index" class="w-full bg-white rounded-lg shadow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500">
          <div>
            <img src="/assets/css/img/gallery/glry.jpg" class="object-center object-cover h-[250px] w-full" :src="item.image" :alt="item.name" />
          </div>
          <div class="text-center py-8 sm:py-6">
            <p class="text-xl text-gray-700 font-bold mb-2">{{ item.name }}</p>
            <p class="text-base text-gray-400 font-normal">{{ item.role }}</p>
          </div>
        </div>
      </div>

      <!-- Tombol Load More -->
      <div class="flex justify-center mt-8" v-if="visibleItems.length < items.length">
        <button class="btn btn-primary" @click="loadMore">Load More</button>
      </div>
    </section>
  </div>
</template>

<style scoped>
.bg {
  background-image: url("/assets/css/img/background/pattern.jpg");
  background-size: cover;
  background-position: center;
  height: 100vh;
}

.hover\:scale-105:hover {
  transform: transition;
}
</style>

<script>
export default {
  data() {
    return {
      // Data Galeri
      items: [
        {
          name: "Porseni",
          role: "21 Desember 2024",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Lucy Carter",
          role: "Graphic Designer",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Jade Bradley",
          role: "Dev Ops",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Mark Johnson",
          role: "Product Manager",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Emily Smith",
          role: "Data Scientist",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Sophia Lee",
          role: "UI/UX Designer",
          image: "/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Dany Bailey",
          role: "Software Engineer",
          image: "/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Lucy Carter",
          role: "Graphic Designer",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Jade Bradley",
          role: "Dev Ops",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Mark Johnson",
          role: "Product Manager",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Emily Smith",
          role: "Data Scientist",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
        {
          name: "Sophia Lee",
          role: "UI/UX Designer",
          image: "@/assets/css/img/gallery/glry.jpg",
        },
      ],

      // Jumlah item yang terlihat
      visibleCount: 6,
    };
  },
  computed: {
    // Data yang akan ditampilkan berdasarkan jumlah visibleCount
    visibleItems() {
      return this.items.slice(0, this.visibleCount);
    },
  },
  methods: {
    // Fungsi untuk menambah jumlah item yang terlihat
    loadMore() {
      this.visibleCount += 3; // Tambahkan 3 item lagi
    },
  },
};
</script>
