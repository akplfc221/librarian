<template>
  <v-app>
    <v-app-bar
      app

    >
      <div class="d-flex align-center">
        <v-img 
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="@/assets/123.jpg"
          transition="scale-transition"
          width="40"
        />
      
       



        {{ $const.APP_NAME }}
      </div>

      <v-spacer></v-spacer>

      <v-btn
        text
      >
        <span class="mr-2">Login</span>
        <v-icon>mdi-account-circle</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style scoped>
@import url('@/assets/styles.css');
</style>
