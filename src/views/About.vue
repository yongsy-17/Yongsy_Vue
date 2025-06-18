<template>
  <div class="p-8">
    <h1 class="text-4xl font-bold text-blue-600 mb-4">Welcome to Yongsy's Vue Website</h1>
    <p class="text-lg text-gray-700 mb-2">
      This is the About page. Here you can find an introduction to our website and what we do.
    </p>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
      <div
        v-for="photo in photos"
        :key="photo.id"
        class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-xl transition-shadow duration-300"
      >
        <img
          :src="photo.url"
          :alt="photo.title"
          class="w-full h-48 object-cover"
          loading="lazy"
        />
        <div class="p-4">
          <h3 class="text-lg font-medium text-gray-900 truncate" :title="photo.title">
            {{ photo.title }}
          </h3>
          <p class="mt-2 text-gray-600 text-sm">
            Delicious food of Cambodia .
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      photos: [
        { id: 1, url: 'src/imges/e740b16ba6d7e506cc082a9994fc1f09.jpg', title: 'papaya salad' },
        { id: 2, url: 'src/imges/2d3f143e99a6989d4a0bcafc4422cda4.jpg', title: 'Oysters Fish Sauce' },
        { id: 3, url: 'src/imges/8e9a74ae20018ab1a962fa2fdce6852f.jpg', title: 'lunch food' },
        { id: 4, url: 'src/imges/9cf565982a851a89c196c31f85f55c44.jpg', title: 'papaya salad' },
        { id: 5, url: 'src/imges/275ab3f8cddc61fa9f19c8459a6c9870.jpg', title: 'Khmer Food' },
        { id: 6, url: 'src/imges/9af4fa8f51c0e4da310f82aeb56dfb72.jpg', title: 'Seafood' },
        { id: 7, url: 'src/imges/e69f66701b584742cc0695ef670048b0.jpg', title: 'Lobsters food' },
        { id: 8, url: 'src/imges/f71dfb8b2da50795ab92a37e2d2ace14.jpg', title: 'Crab Food' },
      ],
    };
  },
};
</script>
