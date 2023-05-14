<template lang="pug">
div
    iframe.planning(src="https://www.figma.com/embed?embed_host=share&amp;url=https%3A%2F%2Fwww.figma.com%2Fproto%2FHwJWx5iK6fZ8rG3TNvnVGw%2FPlanning%3Fnode-id%3D979%253A27%26scaling%3Dcontain%26page-id%3D315%253A2&amp;hide-ui=1" allowfullscreen="allowfullscreen")
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

<style lang="sass">
.planning
  width: 100%
  height: 100%
  margin: auto
html, body
  background-color: black

</style>
