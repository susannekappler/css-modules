<template>
  <div>
    <section>
      <h1>Example 1</h1>
      <InputGroup1 />
    </section>

    <section>
      <h1>Example 2</h1>
      <InputGroup2 />
    </section>
  </div>
</template>

<script>
import InputGroup1 from '@/components/02-Organisms/InputGroup/InputGroupExample1'
import InputGroup2 from '@/components/02-Organisms/InputGroup/InputGroupExample2'

export default {
  name: 'Home',
  components: {
    InputGroup1,
    InputGroup2
  }
}
</script>
