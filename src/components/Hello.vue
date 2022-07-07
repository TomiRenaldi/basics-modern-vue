<script setup>
import { computed } from '@vue/reactivity';

const props = defineProps({
    name: String
})

const upperCase = computed(() => props.name.toLocaleUpperCase())

</script>

<template>
    <div text="red 5xl center" font="mono">Hello, {{upperCase}}</div>
</template>