<template>
    <p v-text="props.msg"></p>
    <slot>Fallback content</slot>
</template>

<script setup>
import { defineEmits, defineProps } from 'vue'

const emit = defineEmits(['response'])

const props = defineProps({
    msg: String
})

emit('response', 'hello from child')
</script>

<style>

</style>