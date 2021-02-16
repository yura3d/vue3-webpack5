<template>
  <button @click="counterIncrement">
    {{ title }}: {{ counter }}
  </button>
</template>

<script>
import { ref } from 'vue'

export default {
  props: {
    title: {
      type: String,
      required: true
    }
  },
  setup () {
    const counter = ref(0)

    const counterIncrement = () => {
      counter.value++
      console.log('New value is', counter.value)
    }

    return {
      counter,
      counterIncrement
    }
  }
}
</script>
