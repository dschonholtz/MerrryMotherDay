<template>
  <transition name="fade" appear>
    <div class="main-content">
      <div class="card mt-3">
        <div class="card--content">
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
            <p>
              Now, if anyone goes to <s>Happy</s>Mother<s>s</s>Day.com. Uh...
              or at least MerryMotherDay.com they will see my note to you :)
            </p>
            <p>
              Sorry I couldn't get HappyMothersDay. It was taken. (And then I misspelled MerryMotherSDay so it isn't plural. Oops)
            </p>
            <p>
              All the same I hope you have a wonderful day.
            </p>
            <p class="signature">Lot's of love,<br>Douglas</p>
        </div>
      </div>
    </div>
  </transition>
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

      &:hover {
          box-shadow: 1rem 1.5rem 4rem rgba(#000, .45);
          transition: box-shadow 0.3s ease-in-out;
      }

      &--content {
          font-family: 'Arizonia';
          font-size: 18px;
          color: #6e6e6e;
          padding: 20px;
          padding-left: 10px;
          padding-right: 10px;
      }
    }

    p {
      text-align: left;

      &.signature {
        padding: 0 20%;
        text-align: right;
      }
    }

    .fade-enter {
        opacity: 0;
        transform: translateY(-1rem);
    }

    .fade-enter-active {
        transition: all .75s ease-in-out;
    }

    s {
      color: red;
    }
</style>
