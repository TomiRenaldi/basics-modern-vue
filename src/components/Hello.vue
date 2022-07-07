<script setup>
import { computed } from '@vue/reactivity';


const props = defineProps({
    name: String
})

const upperCase = computed(() => props.name.toLocaleUpperCase())

</script>

<template>
    <div>Hello, {{upperCase}}</div>
</template>