<template lang="pug">
section.custom-section-streamers
    wave(:rotation="180")
    div
      div.relative.custom-title-streamers.mt-8.mb-12.flex.justify-center
        waves-title.absolute.bottom-0.top-0.custom-streamers-wave-title
        .h1.text-4xl.font-bold.text-center.absolute.text-center.w-full.custom-font-joti_one Les streameurs
      div
        ul.flex.justify-center.streamers
          li.mx-3.flex
            a(target="_blank" href="https://www.twitch.tv/haechi_co")
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/56e556c7-99e4-4a6a-a3f0-9dc542a2d670-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="mw-32 w-32 h-32 mx-auto rounded-full")
          li.mx-3.flex
            a(target="_blank" href="https://www.twitch.tv/samsaouule")
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/bbfa0dd9-cf44-419e-9f04-d9cfb65cd9ce-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="mw-32 w-32 h-32 mx-auto rounded-full")
          li.mx-3.flex
            a(target="_blank" href="https://www.twitch.tv/tacxtv")
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/3430f317-8cbd-4c62-a236-5f3aeafce10d-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="mw-32 w-32 h-32 mx-auto rounded-full")
          li.mx-3.flex
            a(target="_blank" href="https://www.twitch.tv/pazuzuuu_")
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/e3748a06-2640-4888-a0f4-284ddab678b3-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="mw-32w-32 h-32 mx-auto rounded-full")
          li.mx-3.flex
            a(target="_blank" href="https://www.twitch.tv/skypixx")
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/0af9e695-a490-45d5-a057-88ec2d748bb3-profile_image-70x70.jpeg" alt="Logo de la chaîne de streamer" class="mw-32 w-32 h-32 mx-auto rounded-full")
    wave
</template>

<style lang="sass" scoped>
.streamers
  flex-wrap: wrap
.mw-32
  min-width: 8rem
.custom-section-streamers
  background-color: #6441A5

@media (min-width: 1200px)
  .custom-streamers-wave-title, .custom-title-streamers
    height: 120px !important
    .h1
      font-size: 2.5rem !important
      height: 120px !important
      line-height: 120px !important

.custom-streamers-wave-title, .custom-title-streamers
  height: 60px
  .h1
    font-size: 1.5rem
    color: #6441A5
    height: 60px
    line-height: 60px
</style>
