<template>

  <kolibri-nav></kolibri-nav>
  <main>
    <slot></slot>
  </main>
  <footer>
    foot!
  </footer>

</template>

<script>
export default {
  components: {
    'kolibri-nav': require('./navigation.vue'),
  },
};
</script>


<style lang="stylus" scoped>

  @require '~core-theme.styl'

  main
    margin: 10px

  footer
    background-color: $core-bg-light
    bottom: 1vh
    position: fixed
    padding: 10px
    width: 100%

</style>
