<script setup>
import {defineProps} from 'vue'

defineProps({
    tweet: Object,
})

</script>

<template>
    <p class="message">
        {{ tweet.message }}
    </p>
</template>