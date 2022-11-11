<script setup>
import { ref } from 'vue'
import ChildComp from './ChildComp.vue'

const msg = ref('from parent')
const childMsg = ref('No child msg yet')
</script>

<template>
    <ChildComp :msg="msg" @response="(msg) => childMsg = msg">
        <p>Some text</p>
    </ChildComp>

    <p>{{ childMsg }}</p>
</template>