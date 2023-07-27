<template>
    <div style="background-color: grey;" class="grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 xl:gap-x-8">
      <a v-for="product in products" :key="product.id" :href="product.href" class="group">
        <div class="aspect-h-1 aspect-w-1 w-full overflow-hidden rounded-lg bg-gray-200 xl:aspect-h-8 xl:aspect-w-7">
          <img :src="product.imageSrc" :alt="product.imageAlt" class="h-full w-full object-cover object-center group-hover:opacity-75" />
        </div>
        <h3 class="mt-4 text-sm text-gray-700">{{ product.name }}</h3>
        <p class="mt-1 text-lg font-medium text-gray-900">{{ product.price }}</p>
        <p class="mt-1 text-lg font-medium text-gray-900" style="color: black;">{{ product.imageAlt }}</p>
      </a>
    </div>
</template>
<script setup>
const products = [
  {
    id: 1,
    name: 'Jaket Custom GP',
    price: 'Rp. 3.299.000',
    imageSrc: './public/picture/jaket3.jpg',
    imageAlt: 'Dirancang Khusus Untuk Di Gunakan Dalam Balapan Resmi',
  },
  {
    id: 2,
    name: 'Sarung Tangan BMW 44',
    price: 'Rp. 399.000',
    imageSrc: './public/picture/sarung3.jpg',
    imageAlt: 'Menggunakan Bahan Yang Lembut Dan Membuat Nyaman Di Gunakan',
  },
  {
    id: 3,
    name: 'Sarung Tangan BMW Gp 2019',
    price: 'Rp. 14.499.000',
    imageSrc: './public/picture/sarung2.jpg',
    imageAlt: 'Memiliki Bahan Yang Kuat Dan Nyaman Saat Digunakan',
  },
  {
    id: 4,
    name: 'Sarung Tangan Kulit',
    price: 'Rp. 499.000',
    imageSrc: './public/picture/sarung.jpg',
    imageAlt: 'Banyak Digunakan Dalam Balapan Resmi',
  },
]
</script>