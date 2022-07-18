<template>
  <div>
    <input
      :type="type"
      v-model="modelValue"
      @input="handleInput"
    />
  </div>
</template>

<script>
export default {
  name: 'ZzInput',
  inheritAttrs: false,
  props: {
    type: {
      type: String,
      default: 'text'
    },
    modelValue: {
      type: String,
      default: ''
    }
  },
  setup(_props, { emit }) {
    const handleInput = e => {
      emit('update:modelValue', e.target.value)
    }

    return {
      handleInput
    }
  }
}
</script>

<style scoped>

</style>
