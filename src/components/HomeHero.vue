
<template>
  <section class="hero">
    <header>
      <h1 v-text="heroData.name" class="eb-type-h1"></h1>
      <h2 v-text="heroData.position" class="eb-type-h2-alt"></h2>
      <p v-text="heroData.tag"></p>
    </header>
    <ul class="hero__images">
      <li>
        <img class="hero__images__bg" src="/static/img/hero-bg-small.jpg" alt="">
      </li>
    </ul>
  </section>
</template>

<script>
  export default {
    props: ['heroData'],
  };
</script>

<style lang="scss">
@import "../scss/utilities/base";

.hero {
  background: radial-gradient(
    ellipse at center,
    rgba(238, 238, 238, 1) 0%,
    rgba(223, 228, 231, 1) 100%
  );
  margin-top: 45px;
  overflow: hidden;
  @include phone {
    min-height: 40vh;
  }
  position: relative;
  @include skew(left);
  &:after {
    content: "";
    @include full("absolute");
    z-index: z-index(hero2);
    background: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0) 60%,
      rgba(0, 0, 0, 0.5) 100%
    );
  }
  &__images {
    &__txt {
      z-index: z-index(hero1);
    }
    li {
      @include full("absolute");
      max-width: 2000px;
      margin: auto;
      &:last-child {
        position: static;
        opacity: 0;
        animation: opacity 2s linear forwards;
        @include skew(null, 0, -3rem -3em);
      }
    }
    img {
      width: 100%;
      max-width: 100%;

    }
    @include phone {
      img,
      svg {
        max-width: none;
        width: 150%;
      }
    }
    .st0 {
      fill: transparent;
      stroke: $color-dark;
      stroke-miterlimit: 1;
      will-change: stroke-dashoffset;
      stroke-dasharray: 2000;
      stroke-dashoffset: 2000;
      animation: dashHero 5s linear forwards;
    }
    &__camera .st0 {
      animation-delay: 1s;
    }
    &__phone .st0 {
      animation-delay: 2s;
    }
    &__laptop .st0 {
      animation-delay: 3s;
    }
    &__notebook .st0 {
      animation-delay: 4s;
    }
    &__ipad .st0 {
      animation-delay: 5s;
    }
    &__cups .st0 {
      animation-delay: 6s;
    }
    &__keyboard .st0 {
      animation-delay: 5s;
    }
    &__keyboard .st0 {
      animation-delay: 3s;
    }
    /* &__bg {
      opacity: 0;
      animation: opacity 2s linear forwards;
      animation-delay: 6s;
    } */

    .st-fat {
      fill: transparent;
      stroke: $color-dark;
      stroke-width: 2px;
      stroke-miterlimit: 1;
      will-change: stroke-dashoffset;
      stroke-dasharray: 200;
      stroke-dashoffset: 200;
      animation: dashg 0.5s linear forwards;
    }
    $i: 1;
    $add: 0.5;
    $added: 1.5;
    $unit: s;
    @while $i <= 7 {
      .st-fat-#{$i} {
        animation-delay: $added + $add#{$unit};
      }
      $i: $i + 1;
      $added: $added + $add;
    }

    .st-txt {
      fill-opacity: 0;
      animation: show 0.1s linear forwards;
      fill: $color-gray;
    }
    $i2: 1;
    $add2: 0.1;
    $added2: 1;
    $unit2: s;
    @while $i2 <= 12 {
      .st-txt-#{$i2} {
        animation-delay: $added2 + $add2#{$unit};
      }
      $i2: $i2 + 1;
      $added2: $added2 + $add2;
    }
  }
  header {
    position: absolute;
    z-index: z-index(hero3);
    left: 50%;
    transform: translate(-50%, 0);
    @include phone {
      top: 90px;
      width: 80%;
    }
    @include tablet {
      top: 25%;
      width: 90%;
    }
    @include large {
      top: 35%;
    }
    text-align: center;
    line-height: 1;
    text-transform: uppercase;
    opacity: 0;
    animation: opacity 2s linear forwards;
    animation-delay: 2s;
  }
  p {
    font-size: theme-get(text, size, bigger);
    font-weight: theme-get(space, extra);
    margin: theme-get(space, none);
    color: theme-get(text, color, orange);
  }
}
</style>
