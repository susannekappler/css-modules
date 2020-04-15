<template>
  <label
    v-bind="properties"
    :class="$style.baseLabel">{{ text }}</label>
</template>

<script>
export default {
  name: 'BaseLabel',
  props: {
    for: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    }
  },
  data () {
    return {
      properties: {
        type: this.type,
        text: this.text
      }
    }
  }
}
</script>

<style lang="scss" module>
  .baseLabel {
    color: black;
    font-weight: bold;
  }
</style>
