<template>
  <v-app style="
  background-image: url('https://api.fantasyzone.cc/tu')
">
    <v-main style="
    position: absolute;
    top: 0; bottom: 0;
    left: 0; right: 0;
    line-height: 2;
    margin: auto;
    border-radius: 5px;
    background: rgba(255, 255, 255, .6);
    box-shadow: 3px 3px 6px 3px rgba(0, 0, 0, .3);
    overflow: hidden;">
      <router-view/>
    </v-main>
    <v-footer
        color="green"
        style="opacity: 0.5"
        absolute>
      <v-col
          class="text-center"
          style="line-height: normal"
          cols="12"
      >
        Copyright © by HikariLan All Rights Reserved. <a href="https://beian.miit.gov.cn/">陕ICP备2020016655号-1</a>
        <br>
        Powered by Vue.js && Vuetify
        <br>
        The random cover API by <a href="https://api.fantasyzone.cc/">FantasyZone Public API</a>
      </v-col>
    </v-footer>
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
