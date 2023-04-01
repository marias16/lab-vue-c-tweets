<script setup>
import {defineProps} from 'vue'

defineProps({
    tweet: Object,
})

</script>

<template>
    <span class="name">{{  tweet.user.name }}</span>
    <span class="handle">{{ tweet.user.handle }}</span>
</template>