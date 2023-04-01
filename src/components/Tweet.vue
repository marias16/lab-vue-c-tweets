<script setup>
import {defineProps} from 'vue'
import ProfileImage from './ProfileImage.vue'
import UserProfile from './User.vue'
import TimeStamp from './TimeStamp.vue'
import MessageTweet from './Message.vue'
import ActionsTweet from './Actions.vue'

defineProps({
  tweet: Object,
});

</script>

<template>
  <div class="tweet">
    <ProfileImage :tweet="tweet"/>

    <div class="body">
      <div class="top">
        <span class="user">
          <UserProfile :tweet="tweet" />
        </span>
        <TimeStamp :tweet="tweet" />
      </div>

      <MessageTweet :tweet="tweet" />

      <div class="actions">
        <!-- Font Awesome icons -->
        <ActionsTweet />
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
