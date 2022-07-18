<template>
  <div>
    <button @click="handleClick"><slot></slot></button>
  </div>
</template>

<script>
export default {
  name: 'ZzButton',
  inheritAttrs: false,
  setup(_props, { emit }) {
    const handleClick = e => {
      emit('click', e)
      e.preventDefault()
    }

    return {
      handleClick
    }
  }
}
</script>

<style>

</style>
