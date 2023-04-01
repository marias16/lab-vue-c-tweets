<script setup>
import {defineProps} from 'vue'

defineProps({
    tweet: Object,
})
</script>

<template>
    <img
      :src="tweet.user.image"
      class="profile"
      alt="profile"
    />
</template>


