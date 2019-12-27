<template>
  <v-app>
    <AppNavigationBar></AppNavigationBar>
    <v-content>
      <router-view />
    </v-content>
    <v-footer
      app
      color="primary"
      dark>
      Vuetify
    </v-footer>
  </v-app>
</template>

<script>
import AppNavigationBar from './components/AppNavigationBar'

export default {
  components: {
    AppNavigationBar
  },
  data: () => {
    return {
      drawer: null
    }
  }
};
</script>