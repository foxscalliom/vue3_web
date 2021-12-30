<template>
  <div class='home'>
    <div>内容：{{msg}}</div>
  </div>
</template>

<script lang='ts'>
import { ref } from 'vue'
import useCount from '@/views/useCount'

export default {
  name: 'CountDemo',
  setup() {
    const { current: count, inc, dec, set, reset } = useCount(2, {
      min: 1,
      max: 15
    })
    const msg = ref('Demo useCount')

    return {
      count,
      inc,
      dec,
      set,
      reset,
      msg
    }
  }
}
</script>