<template>
<div>
  {{name}}
  {{car.name}}
  {{car.price}}
</div>
</template>

<script setup lang='ts'>
import { ref, reactive } from 'vue'
const  name = ref("李四")
const car = reactive({name:"丰田",price:20})
</script>

<style scoped>

</style>