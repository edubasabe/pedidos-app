<template>
  <nav class="bg-teal-400 flex p-5 mb-6">
    <div class="container mx-auto flex">
      <h2 class="text-white font-bold text-2xl mr-auto">Pedidos App</h2>
      <ul class="flex items-center text-white font-bold">
        <li class="px-3"><nuxt-link to="/">Inicio</nuxt-link></li>
        <li>
          <nuxt-link to="/orders" class="bg-orange-400 rounded py-2 px-3"
            >Haz tu pedido</nuxt-link
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style></style>
