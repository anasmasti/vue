<script setup>
import { reactive, ref } from 'vue'

const counter = reactive({
    count: 0
})
const message = ref('Hello World!')


counter.count++
message.value = 'Changed'
</script>

<template>
    <h1>{{ message.split('').reverse().join('') }}</h1>
    <h1>{{ message }}</h1>
    <p>count is: {{ counter.count }}</p>
</template>