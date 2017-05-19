# vue-twitch-chat [![license](https://img.shields.io/github/license/tserkov/go-twitch-api.svg)]() [![Gemnasium](https://img.shields.io/gemnasium/tserkov/go-twitch-api.svg)]()
A Vue component for embedding Twitch chat. See component for all available properties.

## Install

``` bash
# npm
npm install --save-dev vue-twitch-chat
```

``` bash
# yarn
yarn add --dev vue-twitch-chat
```

## Use (Component)

```html
<template>
  <twitch-chat
    :channel="channel"
  ></twitch-chat>
</template>

<script>
  import VueTwitchChat from 'vue-twitch-chat';

  export default {
    // ...
    components: {
      VueTwitchChat,
    },
    data() {
      return {
        channel: 'tserkov',
      };
    },
    // ...
  };
</script>
```
