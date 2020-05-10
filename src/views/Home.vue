<template>
  <div class="home">
    <HomeTitle msg="Happy Mothers Day"/>
    <HomeContent/>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeTitle from '@/components/HomeTitle.vue'
import HomeContent from '@/components/HomeContent.vue'

export default {
  name: 'Home',
  components: {
    HomeTitle,
    HomeContent
  }
}
</script>

<style lang="scss">
</style>
