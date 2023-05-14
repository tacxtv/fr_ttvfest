<template lang="pug">
section(style="height: 100%")
    twitch-player(channel="TacxTV")
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { definePageMeta } from '#imports'

export default defineComponent({
  name: 'Index',
  setup() {
    definePageMeta({
      layout: 'presentation',
    })
    return {}
  },
})
</script>
