<template lang="pug">
.h-full.w-full
    navbar
    .container.mx-auto.full-without-menu
      lazy-nuxt-page
</template>

<style lang="sass">
.full-without-menu
  height: calc(100vh - 220px)
</style>
