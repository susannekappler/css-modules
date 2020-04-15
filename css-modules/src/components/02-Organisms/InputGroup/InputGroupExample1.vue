<template>
  <InputGroup
    v-bind="inputGroupProperties" />
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
        inputId: 'input1',
        inputPlaceholder: 'Dr. Fauci',
        inputIsDisabled: false,
        inputType: 'text',
        labelFor: 'input1',
        labelText: 'Name'
      }
    }
  }
}
</script>

<style lang="scss" module>

</style>
