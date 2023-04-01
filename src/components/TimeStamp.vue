<script setup>
import {defineProps} from 'vue'

defineProps({
    tweet: Object,
})

</script>

<template>
    <span class="timestamp">{{ tweet.timestamp }}</span>
</template>