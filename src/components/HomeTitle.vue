<template>
  <transition name="fade" appear>
    <div class="home-title">
      <h1>{{ msg }}</h1>
      <video id="flower_video" class="flower-video" autoplay muted @mouseover="videoHover($event.target)">
          <source alt="Pretty Flower Pic I swear" src="../assets/img/animatedBloomingFlower.webm" type="video/webm">
          <source alt="Pretty Flower Pic I swear" src="../assets/img/animatedBloomingFlower.mp4" type="video/mp4">
          Your browser is not supported!
      </video>
    </div>
  </transition>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HomeTitle extends Vue {
  @Prop() private msg!: string;
  videoHover (video: HTMLVideoElement): void {
    video.play()
  }
}
</script>

<style lang="scss">
  h1 {
    font-size: 5rem;
    margin: 40px 0 0;
    color: #e67cc3;
    font-family: antonine_personal_useregular;
  }

    .fade-enter {
        opacity: 0;
        transform: translateY(-1rem);
    }

    .fade-enter-active {
        transition: all .75s ease-in-out;
    }
</style>
