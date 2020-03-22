<template>
  <div class="container mx-auto">
    <div class="flex mb-4">
      <div class="w-1/2 h-12">
        <form action="#" class="flex">
          <BaseInput
            v-model="client.name"
            label="Nombre"
            placeholder="Escribe tu nombre"
            custom-class="w-1/2 mr-6"
          />
          <BaseInput
            v-model="client.phone"
            label="Teléfono"
            placeholder="Escribe tu teléfono"
            custom-class="w-1/2"
          />
        </form>
      </div>
      <div class="w-1/2 h-12 p-5">
        <div class="bg-gray-200 rounded p-5">
          <p>
            <b>Nombre:</b>
            {{ client.name }}
            <br />
            <b>Teléfono:</b>
            {{ client.phone }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BaseInput from '~/components/BaseInput'
export default {
  components: {
    BaseInput
  },
  data: () => {
    return {
      client: {
        name: '',
        phone: ''
      }
    }
  }
}
</script>

<style></style>
