<template lang="pug">
section.custom-section-streamers
    wave(:rotation="180")
    div
      div.relative.custom-title-streamers.mt-8.mb-12.flex.justify-center
        waves-title.absolute.bottom-0.top-0.custom-streamers-wave-title
        .h1.text-4xl.font-bold.text-center.absolute.text-center.w-full.custom-font-joti_one Les streameurs
      div
        ul.flex.justify-center
          li.mx-3
            a
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/3430f317-8cbd-4c62-a236-5f3aeafce10d-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="w-32 h-32 mx-auto rounded-full")
          li.mx-3
            a
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/3430f317-8cbd-4c62-a236-5f3aeafce10d-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="w-32 h-32 mx-auto rounded-full")
          li.mx-3
            a
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/3430f317-8cbd-4c62-a236-5f3aeafce10d-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="w-32 h-32 mx-auto rounded-full")
          li.mx-3
            a
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/3430f317-8cbd-4c62-a236-5f3aeafce10d-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="w-32 h-32 mx-auto rounded-full")
          li.mx-3
            a
              img(src="https://static-cdn.jtvnw.net/jtv_user_pictures/3430f317-8cbd-4c62-a236-5f3aeafce10d-profile_image-70x70.png" alt="Logo de la chaîne de streamer" class="w-32 h-32 mx-auto rounded-full")
    wave
</template>

<style lang="sass" scoped>
.custom-section-streamers
  background-color: #6441A5
.custom-streamers-wave-title, .custom-title-streamers
  height: 120px

  .h1
    color: #6441A5
    height: 120px
    line-height: 120px
</style>
