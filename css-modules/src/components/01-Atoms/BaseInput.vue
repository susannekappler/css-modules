<template>
  <input v-bind="properties">
</template>

<script>

export default {
  name: 'BaseInput',
  props: {
    isDisabled: {
      type: Boolean,
      default: false
    },
    id: {
      type: String,
      required: false
    },
    placeholder: {
      type: String,
      required: false
    },
    type: {
      type: String,
      required: true
    }
  },
  data () {
    return {
      properties: {
        class: 'base-input',
        placeholder: this.placeholder,
        isDisabled: this.isDisabled,
        id: this.id,
        type: this.type
      }
    }
  }
}
</script>

<style lang="scss" scoped>
  .base-input {

  }
</style>
