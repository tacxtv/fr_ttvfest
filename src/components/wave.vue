<template>
  <svg viewBox="0 0 1920 372" fill="none" xmlns="http://www.w3.org/2000/svg" :style="{ transform: `rotate(${rotation}deg)` }">
    <g clip-path="url(#clip0_1_12)">
      <path
        d="M0 0H26.6667C53.3333 0 106.667 0 160 24.8278C213.333 50.1219 266.667 99.0781 320 105.722C373.333 111.9 426.667 74.6 480 74.6C533.333 74.6 586.667 111.9 640 111.9C693.333 111.9 746.667 74.6 800 68.4222C853.333 61.7781 906.667 87.4219 960 118.078C1013.33 149.2 1066.67 186.5 1120 217.622C1173.33 248.278 1226.67 273.922 1280 267.278C1333.33 261.1 1386.67 223.8 1440 174.028C1493.33 124.722 1546.67 61.7781 1600 49.7722C1653.33 37.3 1706.67 74.6 1760 105.722C1813.33 136.378 1866.67 162.022 1893.33 174.028L1920 186.5V373H1893.33C1866.67 373 1813.33 373 1760 373C1706.67 373 1653.33 373 1600 373C1546.67 373 1493.33 373 1440 373C1386.67 373 1333.33 373 1280 373C1226.67 373 1173.33 373 1120 373C1066.67 373 1013.33 373 960 373C906.667 373 853.333 373 800 373C746.667 373 693.333 373 640 373C586.667 373 533.333 373 480 373C426.667 373 373.333 373 320 373C266.667 373 213.333 373 160 373C106.667 373 53.3333 373 26.6667 373H0V0Z"
        fill="url(#paint0_linear_1_12)"
      />
    </g>
    <defs>
      <linearGradient id="paint0_linear_1_12" x1="960" y1="0" x2="960" y2="373" gradientUnits="userSpaceOnUse">
        <stop stop-color="#333333" stop-opacity="0.85" />
        <stop offset="1" stop-color="#333333" />
      </linearGradient>
      <clipPath id="clip0_1_12">
        <rect width="1920" height="373" fill="white" />
      </clipPath>
    </defs>
  </svg>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Wave',
  props: {
    color: {
      type: String,
      default: 'var(--basic-background-color)',
    },
    rotation: {
      type: Number,
      default: 0,
    },
  },
  setup() {
    // defineProps<{
    //   color: String
    // }>()
    return {}
  },
})
</script>
