<template lang="pug">
header.relative.flex.items-center.justify-center.flex-col.bg-cover.custom-hero-bg(class="h-3/5 sm:h-4/5")
      menu-items.absolute.w-full.top-0.z-10.hidden(class="sm:block")
      .absolute.right-0.top-0.z-10(class="xs:block sm:hidden md:hidden lg:hidden xl:hidden")
        icon.w-8.h-8.text-white(name="ic:sharp-menu")
      div.custom-shadow-purple
      img.z-10.custom-hero-logo(src="/hero-logo.png" alt="Background")
      wave.absolute.bottom-0.w-full(preserveAspectRatio="none" height="60px" color="black")
</template>

<style lang="sass" scoped>
  .custom-hero-logo
    width: 200px
    position: absolute
    left: 0
    top: calc(50% - 30px)
    transform: translateY(-50%)
  .custom-hero-bg
    height: 200px
    background-image: url('https://cdn.discordapp.com/attachments/782624831924863027/1107008169600897104/Slide_16_9_-_2_8.png')
    background-position: 0 500px
  .custom-shadow-purple
    position: absolute
    top: 0
    left: 0
    width: 100%
    height: 100%
    background: linear-gradient(180deg, rgba(212, 37, 3, 0.28) 15.22%, rgba(114, 47, 138, 0.54) 100%)
</style>
