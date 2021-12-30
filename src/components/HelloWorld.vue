<template>
  <div class="hello">
    <h2>子组件</h2>
  </div>
</template>

<script lang="ts" setup>
import { inject } from "vue"
const name = inject("name")
console.log(name,'inject') // 沐华
</script>
<style scoped>

</style>
