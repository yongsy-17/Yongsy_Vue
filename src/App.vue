<template>
  <div class="min-h-screen bg-gray-100">
    <nav class="bg-blue-600 p-4 text-white flex gap-8 items-center">
      <router-link to="/" class="flex items-center gap-2 hover:underline">
        <span class="material-icons">home</span>
        Home
      </router-link>
      <router-link to="/about" class="flex items-center gap-2 hover:underline">
        <span class="material-icons">person</span>
        About
      </router-link>
      <router-link to="/contact" class="flex items-center gap-2 hover:underline">
        <span class="material-icons">call</span>
        Contact
      </router-link>
    </nav>
    <main class="p-8">
      <router-view />
    </main>
  </div>
</template>
<script>

</script>
