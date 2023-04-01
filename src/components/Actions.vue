<script setup>
    const classes = ['comment', 'retweet', 'heart', 'share']
</script>

<template>
    <i v-for="classE in classes" :key="classE.id" :class="'far fa-'+classE" />
</template>