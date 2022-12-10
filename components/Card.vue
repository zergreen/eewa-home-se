<template>
  <nuxt-link :to="path">
    <img class="w-full rounded" :src="src" />
    <div class="px-6 pt-4 pb-2 flex">
      <span
        class="bg-red-800 hover:bg-red-900 text-white rounded-full px-3 py-1 text-sm font-semibold mr-2 mb-2 flex"
      >
        <span class="mr-1 text-lg">{{ star }}</span>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 18 18"
          fill="currentColor"
          class="w-5 h-5"
        >
          <path
            fill-rule="evenodd"
            d="M10.868 2.884c-.321-.772-1.415-.772-1.736 0l-1.83 4.401-4.753.381c-.833.067-1.171 1.107-.536 1.651l3.62 3.102-1.106 4.637c-.194.813.691 1.456 1.405 1.02L10 15.591l4.069 2.485c.713.436 1.598-.207 1.404-1.02l-1.106-4.637 3.62-3.102c.635-.544.297-1.584-.536-1.65l-4.752-.382-1.831-4.401z"
            clip-rule="evenodd"
          />
        </svg>
      </span>
      <span
        class="inline-block rounded-full px-3 py-1 text-lg text-gray-500 mr-2 mb-2"
        >{{ ratings }} ratings</span
      >
      <span
        class="inline-block rounded-full px-3 py-1 text-lg font-bold text-gray-700 mr-2 mb-2"
        >{{ name }}</span
      >
    </div>
  </nuxt-link>
</template>

<script>
export default {
  props: {
    ratings: String,
    star: String,
    name: String,
    src: String,
    path: String,

  },
};
</script>
