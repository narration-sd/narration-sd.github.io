<template>
  <v-app>
    <Nav/>
    <v-content>
      <v-container>
        <slot/>
      </v-container>
    </v-content>
  </v-app>
</template>

<static-query>
  query {
    metadata {
              siteName
    }
  }
</static-query>

<script>
  import Nav from '~/components/Nav.vue'

  export default {
    components: {
      "Nav": Nav
    }
  }
</script>

<style>

</style>
