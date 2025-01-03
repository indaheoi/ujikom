<template>
    <!-- component -->
     <div class="bg-blue-100">
 <section class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-4 py-12">
    <div class="text-center pb-12">
        <h1 class="font-bold text-3xl md:text-4xl lg:text-5xl font-heading text-gray-900">
            Check our awesome team members
        </h1>
    </div>
    <!-- foto 1 -->
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div class="w-full bg-white rounded-lg sahdow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500">
            <div>
                <img class="object-center object-cover h-[250px] w-full" src="/" alt="photo">
            </div>
            <div class="text-center py-8 sm:py-6">
                <p class="text-xl text-gray-700 font-bold mb-2">Dany Bailey</p>
                <p class="text-base text-gray-400 font-normal">Software Engineer</p>
            </div>
        </div>
        <!-- foto 2 -->
        <div class="w-full bg-white rounded-lg sahdow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500">
            <div>
                <img class="object-center object-cover h-auto w-full" src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1170&q=80" alt="photo">
            </div>
            <div class="text-center py-8 sm:py-6">
                <p class="text-xl text-gray-700 font-bold mb-2">Lucy Carter</p>
                <p class="text-base text-gray-400 font-normal">Graphic Designer</p>
            </div>
        </div>
        <!-- foto 3 -->
        <div class="w-full bg-white rounded-lg sahdow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500">
            <div>
                <img class="object-center object-cover h-auto w-full" src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1171&q=80" alt="photo">
            </div>
            <div class="text-center py-8 sm:py-6">
                <p class="text-xl text-gray-700 font-bold mb-2">Jade Bradley</p>
                <p class="text-base text-gray-400 font-normal">Dev Ops</p>
            </div>
        </div>
        <!-- foto 4 -->
        <div class="w-full bg-white rounded-lg sahdow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500">
            <div>
                <img class="object-center object-cover h-auto w-full" src="https://images.unsplash.com/flagged/photo-1570612861542-284f4c12e75f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1170&q=80" alt="photo">
            </div>
            <div class="text-center py-8 sm:py-6">
                <p class="text-xl text-gray-700 font-bold mb-2">Dany Bailey</p>
                <p class="text-base text-gray-400 font-normal">Software Engineer</p>
            </div>
        </div>
        <!-- foto 5 -->
        <div class="w-full bg-white rounded-lg sahdow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500">
            <div>
                <img class="object-center object-cover h-auto w-full" src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1170&q=80" alt="photo">
            </div>
            <div class="text-center py-8 sm:py-6">
                <p class="text-xl text-gray-700 font-bold mb-2">Lucy Carter</p>
                <p class="text-base text-gray-400 font-normal">Graphic Designer</p>
            </div>
        </div>
        <!-- foto 6 -->
        <div class="w-full bg-white rounded-lg sahdow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500">
            <div>
                <img class="object-center object-cover h-auto w-full" src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1171&q=80" alt="photo">
            </div>
            <div class="text-center py-8 sm:py-6">
                <p class="text-xl text-gray-700 font-bold mb-2">Jade Bradley</p>
                <p class="text-base text-gray-400 font-normal">Dev Ops</p>
            </div>
        </div>
    </div>

    <section class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-4 py-12">
    <div class="text-center pb-12">
      <h1 class="font-bold text-3xl md:text-4xl lg:text-5xl text-gray-900">
        Check our awesome team members
      </h1>
    </div>

    <!-- Galeri Grid -->
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 gap-6">
      <!-- Render galeri secara dinamis -->
      <div
        v-for="(item, index) in visibleItems"
        :key="index"
        class="w-full bg-white rounded-lg shadow-lg overflow-hidden flex flex-col justify-center items-center hover:scale-105 transform transition-all duration-500"
      >
        <div>
          <img src="/assets/css/img/gallery/glry.jpg" alt="Static Image"
          

            class="object-center object-cover h-[250px] w-full"
            :src="item.image"
            :alt="item.name"
          />
        </div>
        <div class="text-center py-8 sm:py-6">
          <p class="text-xl text-gray-700 font-bold mb-2">{{ item.name }}</p>
          <p class="text-base text-gray-400 font-normal">{{ item.role }}</p>
        </div>
      </div>
    </div>

    <!-- Tombol Load More -->
    <div class="flex justify-center mt-8" v-if="visibleItems.length < items.length">
      <button
        class="btn btn-primary"
        @click="loadMore"
      >
        Load More
      </button>
    </div>
  </section>
  </section>
</div>
<div>
  </div>

</template>

<style scoped>
.bg-blue-100{
    background-image: url('/assets/css/img/background/pattern.jpg');
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
          role: "Software Engineer",
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