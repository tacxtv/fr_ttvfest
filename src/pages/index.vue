<template lang="pug">
div.h-full.w-full.accueil
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

<style lang="sass">
.accueil
  background-color: var(--basic-background-color)
</style>
