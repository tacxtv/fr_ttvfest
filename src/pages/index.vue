<template lang="pug">
div.h-full.w-full
    section-presentation
    section-streamers
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { definePageMeta } from '#imports'

export default defineComponent({
  name: 'Index',
  setup() {
    definePageMeta({
      layout: 'onepage',
    })
    return {}
  },
})
</script>
