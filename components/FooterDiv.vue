<template>
  <footer>🥺 <a href="https://github.com/osawa-koki" target="_blank">@osawa-koki</a> 🥺</footer>
</template>

<script>
import pages from '~/pages';

export default {
  name: 'HeaderDiv',
  data() {
    return {
      pages,
    }
  },
}
</script>

<style lang="scss" scoped>
footer {
  height: 70px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: lightgray;
}
</style>

