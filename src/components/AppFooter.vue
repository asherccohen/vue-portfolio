<template>
  <footer class="main-footer">
    <div class="main-footer__wrap">
      <p><small>Designed and Coded with <span>&#10084;</span> by <span>Asher C. Cohen</span> 2019.</small></p>
      <p><small>The code repo for this page can be found <span>@</span><a href="https://github.com/">https://github.com/asherccohen/portfolio-vue-master</a></small></p>

      <p class="dark"><small>Source Technology used: SVG + HTML + SCSS + JS + VueJS + Firebase + GitHub.</small></p>
      <p class="dark"><small>Stock Photography courtesy of https://picjumbo.com.</small></p>
      <p class="dark"><small>Header image courtesy of <a href="https://www.freepik.com/free-photo/wooden-tabletop-at-tropical-paper-texture-wall-template-mock-up-for-display-of-product-business-presentation_1381339.htm">Tirachard</a>.</small></p>
    </div>
  </footer>
</template>

<script>
  import EbMedia from '@/components/EbMedia';

  export default {
    components: {
      EbMedia,
    },
  };
</script>

<style lang="scss">
@import "../scss/utilities/base";

.main-footer {
	margin: auto;
	overflow: hidden;
	position: relative;
  &__wrap {
    background-color: theme-get(background, alternate);
    @include skew(right, null, null);

    @include phone {
      padding: theme-get(space, big);
    }
    @include tablet {
      padding: theme-get(space, bigger);
    }
    @include large {
      padding-top: theme-get(space, bigger);
      padding-bottom: theme-get(space, bigger);
      padding-left: theme-get(space, huge);
      padding-right: theme-get(space, huge);
    }
  }
  .logo {
    width: 150px;
    @include phone {
      width: 110px;
    }
    @include tablet {
      width: 130px;
    }
    @include large {
      width: 150px;
    }
  }
  p {
    margin-bottom: theme-get(space, none);
    span {
      color: $color-light;
    }
    &.dark {
      color: $color-blue;
      margin-top: theme-get(space, normal);
      font-size: theme-get(text, size, small);
      &:last-child {
        margin-top: theme-get(space, none);
      }
    }
  }
}
</style>
