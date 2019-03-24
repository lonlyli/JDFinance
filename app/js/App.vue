<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>
<style lang="scss">
.router-link-exact-active{
  p{
    color: red !important;
  }
}
</style>
