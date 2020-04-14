<template>
  <div id="app">
    <InputGroup
      v-bind="inputGroupProperties"
      :class="$style.inputGroup" />
    <router-view/>
  </div>
</template>

<script>
import InputGroup from '@/components/02-Organisms/InputGroup'

export default {
  name: 'app',
  components: {
    InputGroup
  },
  data () {
    return {
      inputGroupProperties: {
        inputId: 'base-input',
        inputPlaceholder: 'Philanthrope',
        inputIsDisabled: false,
        inputType: 'text',
        labelFor: 'base-input',
        labelText: 'Name'
      }
    }
  }
}

</script>
<style lang="scss" module>
  @import "@/styles/global.scss";

  .inputGroup {
    border: 3px solid orange;
  }
</style>
