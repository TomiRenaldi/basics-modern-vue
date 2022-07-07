<script setup>
import { computed } from '@vue/reactivity';

const props = defineProps({
    name: String
})

const upperCase = computed(() => props.name.toLocaleUpperCase())

</script>

<template>
    <div text="red 5xl" font-sans>Hello, {{upperCase}}</div>
    <div i-carbon-bee text-5xl></div>
</template>