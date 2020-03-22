<template>
  <label class="input-group" :class="customClass">
    <p class="text-sm mb-2 text-gray-600">{{ label }}</p>
    <input
      class="bg-white focus:outline-none focus:shadow-outline border border-gray-300 rounded-lg py-2 px-4 block w-full appearance-none leading-normal"
      v-bind="$attrs"
      :value="value"
      @input="$emit('input', $event.target.value)"
    />
  </label>
</template>

<script>
export default {
  inheritAttrs: false,
  props: {
    value: {
      type: String,
      default: ''
    },
    label: {
      type: String,
      default: 'Nombre'
    },
    customClass: {
      type: String,
      default: 'w-1/2'
    }
  }
}
</script>

<style></style>
