<template>
  <iframe
    :src="src"
    :width="width"
    :height="height"
    :frameborder="frameBorder"
    :scrolling="scrolling"
  ></iframe>
</template>

<script>
  export default {
    name: 'twitch-chat',
    props: {
      channel: {
        type: String,
        required: true,
      },
      frameBorder: {
        type: Number,
        default: 0,
      },
      width: {
        type: String,
        default: '200',
      },
      height: {
        type: String,
        default: '300',
      },
      scrolling: {
        type: Boolean,
        default: true,
      },
    },
    computed: {
      src() {
        return `//www.twitch.tv/${this.channel}/chat`;
      },
    },
  };
</script>
