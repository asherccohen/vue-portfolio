<template>
  <header class="main-header">
    <eb-media></eb-media>
  </header>
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

.main-header {
  @include full();
  bottom: auto;
  z-index: z-index(header);
  background-color: theme-get(background, alternate);
  text-align: center;
  height: 35px;
  padding-top: theme-get(space, small);
  .logo {
    width: 60px;
    margin-left: theme-get(space, small);;
  }
}
</style>
