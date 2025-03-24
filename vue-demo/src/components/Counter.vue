<!-- src/components/Counter.vue -->
<script setup>
import { ref } from 'vue'

// 定义一个响应式变量
const count = ref(0)

// 方法：增加计数
const increment = () => {
  count.value++
}

// 方法：减少计数
const decrement = () => {
  count.value--
}
</script>

<template>
  <div class="counter">
    <h1>Vue 3 计数器示例 v1 xpp 88877777</h1>
    <p>当前计数: {{ count }}</p>
    <button @click="increment">增加</button>
    <button @click="decrement">减少</button>
  </div>
</template>

<style scoped>
.counter {
  text-align: center;
  margin-top: 50px;
}
button {
  margin: 10px;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}
</style>
