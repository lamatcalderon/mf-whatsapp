<template>
  <div class="image-message">
    <div class="image">
        <img :src="`data:image/png;base64,${multimediaMessage.preview}`"/>
        <span v-if="multimediaMessage?.messageContent" class="message-history-text">{{ multimediaMessage.messageContent }}</span>
        <div class="space-message-history"></div>
    </div>
  </div>
</template>

<script src="./image-message.ts" lang="ts"/>
<style src="./image-message.scss" lang="scss" scoped/>