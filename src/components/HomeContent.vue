<template>
  <div class="main-content">
    <div class="card card-default mt-3">
      <div class="card-content">
          <p>
            Dear Momma,
          </p>
          <p>
            Thanks for being a great mom. You always have encouraged me to do the practical
            thing. But at the same time to chase what I want to do.
          </p>
          <p>
            This year, I wanted to make you something and shout how much I appreciate you
            from the top of a mountain. Unfortunately, Covid makes getting to mountains
            difficult, so I made you this website instead.
          </p>
          <p class="signature">Lot's of love,<br>Douglas</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component
export default class HomeContent extends Vue {
}
</script>

<style lang="scss" scoped>
    .card {
      border: none;
      border-radius: 10px;
      width: 75%;
      margin: 0 auto;
      box-shadow: 1rem 1.5rem 4rem rgba(#000, .1);
    }
    .card-body {
        font-family: 'Arizonia';
        font-size: 18px;
        color: #6e6e6e;
        padding: 20px;
    }

    .card:hover {
        box-shadow: 1rem 1.5rem 4rem rgba(#000, .45);
        transition: box-shadow 0.3s ease-in-out;
    }

    .card-content {
        padding-left: 10px;
        padding-right: 10px;
    }
    p {
      text-align: left;

      &.signature {
        padding: 0 20%;
        text-align: right;
      }
    }
</style>
