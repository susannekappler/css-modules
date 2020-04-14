<template>
  <div :class="$style.inputGroup">
    <BaseLabel
      v-bind="labelProperties"
      :class="$style.baseLabel" />
    <BaseInput
      v-bind="inputProperties"
      :class="$style.baseInput" />
  </div>
</template>

<script>
import BaseLabel from '@/components/01-Atoms/BaseLabel'
import BaseInput from '@/components/01-Atoms/BaseInput'

export default {
  name: 'InputGroup',
  components: {
    BaseLabel,
    BaseInput
  },
  props: {
    labelFor: {
      type: String,
      required: true
    },
    labelText: {
      type: String,
      required: true
    },
    inputId: {
      type: String,
      required: true
    },
    inputType: {
      type: String,
      required: true
    },
    inputPlaceholder: {
      type: String
    },
    inputIsDisabled: {
      type: Boolean
    }
  },
  data () {
    return {
      inputProperties: {
        type: this.inputType,
        id: this.inputId,
        placeholder: this.inputPlaceholder,
        isDisabled: this.inputIsDisabled
      },
      labelProperties: {
        for: this.labelFor,
        text: this.labelText
      }
    }
  }
}
</script>

<style lang="scss" module>
  .inputGroup {
    border: 1px solid green;
    padding: 10px;
  }

  .baseLabel,
  .baseInput {
    display: block;
    width: 400px;;
  }

  .baseInput {
    margin-top: 5px;
  }
</style>
