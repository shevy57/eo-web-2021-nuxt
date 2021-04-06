<template>
  <v-footer color="" padless class="bg-transparent px-md-16 px-0 py-5">
    <v-row justify="center" no-gutters class="px-md-12 px-6">
      <v-col cols="12" md="6" class="text-md-left text-center my-auto">
        <nuxt-link
          to=""
          v-for="link in links"
          :key="link"
          elevation="0"
          rounded
          class="my-2 bg-transparent text-decoration-none text-uppercase"
        >
          {{ link }}
        </nuxt-link>
      </v-col>

      <v-col
        class="py-4 text-md-right text-center dark--text font-weight-light"
        cols="12"
        md="6"
      >
        @ {{ new Date().getFullYear() }}, made with by <v-icon class="">mdi-cards-heart</v-icon> 
        <span class="purple--text">Creative tim</span> for a better web.
      </v-col>
    </v-row>
  </v-footer>
</template>
<script>
export default {
  data() {
    return {
      links: ['creative tim', 'About Us', 'blog', 'licenses'],
    }
  },
}
</script>
<style scoped>
.bg-transparent {
  background-color: transparent !important;
}
.tex-grety {
  color: #999;
}
.v-application a {
  color: #3c4858 !important;
  padding: 0.9375rem;
  font-size: 12px;
  font-weight: 500;
  border-radius: 3px;
  text-transform: uppercase;
  text-decoration: none;
}
.v-application a:hover {
  color: #9c27b0 !important;
}
</style>