<script setup>
import { ref } from 'vue'
let username = ref("")


</script>



<template>
    This is a template 123213213
    <textarea v-model="username"></textarea>


    USERNAME: {{ username }}
</template>