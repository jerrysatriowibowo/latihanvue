<template>
    <br><h1><center>𝑷𝒓𝒐𝒅𝒖𝒌 𝑳𝒂𝒊𝒏</center></h1>
        <br><div style="background-color: grey;" class="grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 xl:gap-x-8">
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
    name: 'Jaket Balap',
    price: 'Rp. 1.990.000',
    imageSrc: './picture/jaket1.jpg',
    imageAlt: 'Di Desain Untuk Rideing Sehari-hari Terbuat Dari Bahan Yang Elastis',
  },
  {
    id: 2,
    name: 'Jaket Model1 OEM',
    price: 'Rp. 299.000',
    imageSrc: './picture/jaket2.webp',
    imageAlt: 'Bisa Digunakan Untuk Berkendara Sehari-hari Terbuat Dari Bahan Yang Dingin',
  },
  {
    id: 3,
    name: 'Jaket Model2 OEM',
    price: 'Rp. 799.000',
    imageSrc: './picture/jaket5.webp',
    imageAlt: 'Bisa Digunakan Untuk Berkendara Sehari-hari Terbuat Dari Bahan Yang Dingin',
  },
  {
    id: 4,
    name: 'Jaket Custom 44',
    price: 'Rp. 120.000',
    imageSrc: './picture/jaket4.jpg',
    imageAlt: 'Menggunakan Bahan Yang Membuat Pengguna Merasa Sejuk',
  },
]
</script>