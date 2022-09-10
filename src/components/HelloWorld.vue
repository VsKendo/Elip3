<template>
  <div class="hello">
    <h1>{{ value }}</h1>
    <button @click="onClick">add</button>
  </div>
</template>

<script lang="ts" setup>
import { onMounted, ref } from 'vue'
import { api } from '@/api/post'

type a = {
  a: string
}
type b = {
  b: string
}
const val = ref()
onMounted(async () => {
  val.value = api()
})
const values = ref<Array<b & a>>([])
const onClick = () => {
  values.value.push(1)
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
