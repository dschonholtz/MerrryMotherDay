<template>
  <div class="main-content">
    <h1>{{ msg }}</h1>
    <p class="hello__mom">
      Happy Mothers Day Mom!
      I hope it is a good one :)
      I love you lots and you mean the world to me.
    </p>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HomeContent extends Vue {
  @Prop() private msg!: string;
}
</script>

<style lang="scss">
h1 {
  margin: 40px 0 0;
}
</style>
