<template>
  <br><h1><center>𝑭𝒍𝒂𝒔𝒉 𝑺𝒂𝒍𝒆</center></h1>
      <br><div style="background-color: grey;" class="grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 xl:gap-x-8">
        <a v-for="product in products" :key="product.id" :href="product.href" class="group">
          <div class="aspect-h-1 aspect-w-1 w-full overflow-hidden rounded-lg bg-gray-200 xl:aspect-h-8 xl:aspect-w-7">
            <img :src="product.imageSrc" :alt="product.imageAlt" class="h-full w-full object-cover object-center group-hover:opacity-75" />
          </div>
          <h3 class="mt-4 text-sm text-gray-700">{{ product.name }}</h3>
          <p class="line-through" style="color: red;">{{ product.fake }}</p>
          <p class="mt-1 text-lg font-medium text-gray-900">{{ product.price }}</p>
        </a>
      </div>
</template>
<script setup>
const products = [
  {
    id: 1,
    name: 'AGV Pista GP RR',
    fake: 'Rp. 29.190.000',
    price: 'Rp. 28.490.000',
    imageSrc: './public/picture/agv.webp',
    imageAlt: 'Tall slender porcelain bottle with natural clay textured body and cork stopper.',
  },
  {
    id: 2,
    name: 'New KYT R2R',
    fake: 'Rp. 2.490.000',
    price: 'Rp. 2.349.000',
    imageSrc: './public/picture/agv.webp',
    imageAlt: 'Olive drab green insulated bottle with flared screw lid and flat top.',
  },
  {
    id: 3,
    name: 'KYT TT Course',
    fake: 'Rp. 1.520.000',
    price: 'Rp. 1.449.000',
    imageSrc: './public/picture/agv.webp',
    imageAlt: 'Person using a pen to cross a task off a productivity paper card.',
  },
  {
    id: 4,
    name: 'New Shoe Helmet',
    fake: 'Rp. 14.600.000',
    price: 'Rp. 14.399.000',
    imageSrc: './public/picture/agv.webp',
    imageAlt: 'Hand holding black machined steel mechanical pencil with brass tip and top.',
  },
]
</script>