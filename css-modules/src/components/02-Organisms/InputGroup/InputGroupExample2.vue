<template>
  <InputGroup
    v-bind="inputGroupProperties"
    :class="$style.inputGroup" />
</template>

<script>
import InputGroup from '@/components/02-Organisms/InputGroup/InputGroup'

export default {
  name: 'InputGroupExample1',
  components: {
    InputGroup
  },
  data () {
    return {
      inputGroupProperties: {
        inputId: 'input2',
        inputPlaceholder: 'The Pope',
        inputIsDisabled: false,
        inputType: 'text',
        labelFor: 'input2',
        labelText: 'Title'
      }
    }
  }
}
</script>

<style lang="scss" module>
  .inputGroup {
    background-color: lavender;
  }
</style>
