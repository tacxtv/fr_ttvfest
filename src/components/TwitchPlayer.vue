<template lang="pug">
div(ref="player" :style="{height: '100%'}")
</template>

<script>
let player

//https://dev.twitch.tv/docs/embed/everything#logging-in
// noinspection JSUnusedGlobalSymbols
export default {
  name: 'TwitchPlayer',
  props: {
    width: {
      type: String,
      default: '100%',
    },
    height: {
      type: String,
      default: '100%',
    },
    volume: {
      type: Number,
      default: 0.5,
    },
    quality: {
      type: String,
      default: 'medium',
    },
    playsInline: {
      type: Boolean,
      default: false,
    },
    channel: String,
    collection: String,
    video: String,
  },
  watch: {
    channel(newChannel) {
      player.setChannel(newChannel)
    },

    collection(newCollection) {
      player.setCollection(newCollection)
    },

    video(newVideo) {
      player.setVideo(newVideo)
    },

    volume(newVolume) {
      player.setVolume(newVolume)
    },
    quality(newQuality) {
      if (player.getQualities().indexOf(newQuality) !== -1) {
        player.setQuality(newQuality)
      }
    },
  },
  methods: {
    play() {
      player.play()
    },

    pause() {
      player.pause()
    },

    seek(timestamp) {
      player.seek(timestamp)
    },

    getCurrentTime() {
      return player.getCurrentTime()
    },

    getDuration() {
      return player.getDuration()
    },

    getPlaybackStats() {
      return player.getPlaybackStats()
    },

    getQuality() {
      return player.getQuality()
    },

    isPaused() {
      return player.isPaused()
    },

    hasEnded() {
      return player.getEnded()
    },

    getVolume() {
      return player.getVolume()
    },

    isMuted() {
      return player.getMuted()
    },

    mute() {
      player.setMuted(true);
    },

    unmute() {
      player.setMuted(false)
    },

    checkChannel() {
      return this.channel === player.getChannel()
    },

    checkVideo() {
      return this.video = player.getVideo()
    },
  },
  beforeCreate() {
    this.$loadScript('//player.twitch.tv/js/embed/v1.js')
      .then(() => {
        const options = {
          width: this.width,
          height: this.height,
          layout: 'video-with-chat',
        }
        if (this.playsInline) {
          options.playsinline = true;
        }

        if (this.channel) {
          options.channel = this.channel;
        } else if (this.collection) {
          options.collection = this.collection;
        } else if (this.video) {
          options.video = this.video;
        } else {
          this.$emit('error', 'no source specified');
        }
        player = new window.Twitch.Embed(this.$refs.player, options)
        player.addEventListener('ended', () => this.$emit('ended'))
        player.addEventListener('pause', () => this.$emit('pause'))
        player.addEventListener('play', () => this.$emit('play'))
        player.addEventListener('offline', () => this.$emit('offline'))
        player.addEventListener('online', () => this.$emit('online'))
        player.addEventListener('ready', () => {
          player.setQuality(this.quality)
          player.setVolume(this.volume)
          this.$emit('ready')
        })
      })
      .catch((e) => this.$emit('error', e))
  }
}
</script>

<style scoped>
</style>
