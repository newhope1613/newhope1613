<script setup>
let props = defineProps(
    {
        name: String,  // Only String
        age: [Number, String],  // Number or String
    }
)
</script>


<template>
    MyProps: {{ props.name }} {{ props.age }}
</template>