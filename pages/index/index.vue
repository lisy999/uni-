<template>
<div>
  {{name}}
  {{car.name}}
  {{car.price}}
  <button @click="changeName">改变名字</button>
</div>
</template>

<script setup lang='ts'>
import { ref, reactive } from 'vue'
const name = ref("李四")
const car = reactive({name:"丰田",price:20})
	
const changeName = ()=>{
	name.value= "王五"
}
</script>

<style scoped>

</style>