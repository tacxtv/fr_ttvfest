<template lang="pug">
header.relative.flex.items-center.justify-center.flex-col.bg-cover.custom-hero-bg(class="h-3/5 sm:h-4/5 md:h-full")
    menu-items.absolute.w-full.top-0.z-10.hidden(class="sm:block")
    .absolute.right-0.top-0.z-10(class="xs:block sm:hidden md:hidden lg:hidden xl:hidden")
      icon.w-8.h-8.text-white(name="ic:sharp-menu")
    div.custom-shadow-purple
    img.z-10.custom-hero-logo(src="/hero-logo.png" alt="Background")
    wave.absolute.bottom-0.w-full
</template>

<style lang="sass" scoped>
  .custom-hero-logo
    width: 80vh
    margin-top: -120px
  .custom-hero-bg
    background-image: url('https://media.discordapp.net/attachments/1029010150226399262/1054008382719270983/IMG_0537.jpg')
  .custom-shadow-purple
    position: absolute
    top: 0
    left: 0
    width: 100%
    height: 100%
    background: linear-gradient(180deg, rgba(212, 37, 3, 0.28) 15.22%, rgba(114, 47, 138, 0.54) 100%)
</style>
