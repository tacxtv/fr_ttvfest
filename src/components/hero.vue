<template lang="pug">
header.relative.flex.items-center.justify-center.flex-col.bg-cover.custom-hero-bg(class="h-3/5 sm:h-4/5 md:h-full custom-hero-bg-desktop")
    menu-items.absolute.w-full.top-0.z-10.hidden(class="sm:block")
    .absolute.right-0.top-0.z-10(class="xs:block sm:hidden md:hidden lg:hidden xl:hidden")
      icon.w-8.h-8.text-white(name="ic:sharp-menu")
    div.custom-shadow-purple
    img.z-10.custom-hero-logo(src="/hero-logo.png" alt="Background")
    wave.absolute.bottom-0.w-full(preserveAspectRatio="none" height="20vh")
</template>

<style lang="sass" scoped>
  .custom-hero-logo
    position: absolute
    width: 80vh
    margin-botoom: -120px
  .custom-hero-bg
    background: url('https://cdn.discordapp.com/attachments/782624831924863027/1107008169600897104/Slide_16_9_-_2_8.png') 0% 0% repeat
    background-size: cover
    background-position: center
    animation-name: MOVE-BG
    animation-duration: 20s
    animation-timing-function: linear
    animation-iteration-count: infinite
    animation-direction: alternate
  .custom-shadow-purple
    position: absolute
    top: 0
    left: 0
    width: 100%
    height: 100%
    background: linear-gradient(180deg, rgba(212, 37, 3, 0.28) 15.22%, rgba(114, 47, 138, 0.54) 100%)

  @keyframes MOVE-BG
    from
      background-position: 0% 0%
    to
      background-position: 60vw 0%

  @media (min-width: 768px)
    .custom-hero-bg-desktop
      animation-name: MOVE-BG-DESKTOP
    @keyframes MOVE-BG-DESKTOP
      from
        background-position: 0% 0%
      to
        background-position: 200% 0%
  @media (min-width: 1480px)
    .custom-hero-bg-desktop
      animation-name: MOVE-BG-DESKTOP-LARGE
    @keyframes MOVE-BG-DESKTOP-LARGE
      from
        background-position: 0% 0%
      to
        background-position: 60vw 0%
</style>
