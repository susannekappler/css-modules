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
    // @include set-text-properties($theme-copy-label, copy);
    color: red;
  }
</style>
