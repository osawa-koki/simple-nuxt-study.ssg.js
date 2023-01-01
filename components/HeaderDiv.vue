<template>
  <header>
    <nav>
      <ul>
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

