<script setup lang="ts">
import { onMounted, ref } from 'vue'
import type { Ref } from 'vue'
import Upload from './components/v-upload/VUpload.vue'
const name: Ref<string> = ref('hhh')

interface Res {
  successful: Boolean
  resultValue: any
}
const res: Ref<Res> = ref({ successful: true, resultValue: [] })

onMounted(() => {
  console.log(name)
  const arr = [1, 2, 3, 0]
  const hasLogin = 3 / 2 === 1
  arr.forEach((item) => {
    console.log(item)
  })
})
</script>

<template>
  <div> vue3 </div>
</template>

<style lang="less" scoped>

</style>
