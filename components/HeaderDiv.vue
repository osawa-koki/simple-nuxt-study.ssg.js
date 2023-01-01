<template>
  <header>
    <nav>
      <ul id="Links">
        <li v-for="page in pages" :key="page.name">
          <nuxt-link :to="page.path">
            {{ page.name }}
          </nuxt-link>
        </li>
      </ul>
    </nav>
  </header>
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

<style lang="scss">
#Links {
  margin-top: 3rem;
  display: flex;
  a {
    margin-right: 0.5rem;
    margin-bottom: 1rem;
    padding-right: 0.5rem;
    border-right: 1px lightgray solid;
    color: #0E6DFE;
    text-decoration: none;
    &:last-child {
      margin-right: 0;
      padding-right: 0;
      border-right: none;
    }
    &:hover {
      text-decoration: underline;
    }
  }
}
</style>

