<template>
      <div style="background-color: rgb(202, 202, 202);" class="grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 xl:gap-x-8">
        <a v-for="product in products" :key="product.id" :href="product.href" class="group">
          <div class="aspect-h-1 aspect-w-1 w-full overflow-hidden rounded-lg bg-gray-200 xl:aspect-h-8 xl:aspect-w-7">
            <img :src="product.imageSrc" :alt="product.imageAlt" class="h-full w-full object-cover object-center group-hover:opacity-75" />
          </div>
          <h3 class="mt-4 text-sm text-gray-700">{{ product.name }}</h3>
          <p class="mt-1 text-lg font-medium text-gray-900">{{ product.price }}</p>
        </a>
      </div>
</template>
<script setup>
const products = [
  {
    id: 1,
    name: 'AGV KSV3',
    price: 'Rp. 3.299.000',
    imageSrc: './picture/agv.webp',
    imageAlt: 'Tall slender porcelain bottle with natural clay textured body and cork stopper.',
  },
  {
    id: 2,
    name: 'New INK Helmet',
    price: 'Rp. 399.000',
    imageSrc: './picture/agv.webp',
    imageAlt: 'Olive drab green insulated bottle with flared screw lid and flat top.',
  },
  {
    id: 3,
    name: 'Helm Bogo',
    price: 'Rp. 120.000',
    imageSrc: './picture/agv.webp',
    imageAlt: 'Person using a pen to cross a task off a productivity paper card.',
  },
  {
    id: 4,
    name: 'New KYT Helmet',
    price: 'Rp. 799.000',
    imageSrc: './picture/agv.webp',
    imageAlt: 'Hand holding black machined steel mechanical pencil with brass tip and top.',
  },
]
</script>