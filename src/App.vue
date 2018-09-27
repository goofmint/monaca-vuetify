<template>
  <v-app>
    <v-navigation-drawer app></v-navigation-drawer>
    <v-toolbar app></v-toolbar>
    <v-content>
      <v-container fluid>

    <v-toolbar
      color="primary"
      dark
    >
      <v-toolbar-side-icon></v-toolbar-side-icon>

      <v-toolbar-title class="white--text">Title</v-toolbar-title>

      <v-spacer></v-spacer>


      <v-btn icon>
        <v-icon>refresh</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>more_vert</v-icon>
      </v-btn>
    </v-toolbar>

              <v-btn-toggle v-model="toggle_exclusive">
                <v-btn flat>
                  <v-icon>format_align_left</v-icon>
                </v-btn>
                <v-btn flat>
                  <v-icon>format_align_center</v-icon>
                </v-btn>
                <v-btn flat>
                  <v-icon>format_align_right</v-icon>
                </v-btn>
                <v-btn flat>
                  <v-icon>format_align_justify</v-icon>
                </v-btn>
              </v-btn-toggle>
        <router-view>
        </router-view>
      </v-container>
    </v-content>
    <v-footer app></v-footer>
  </v-app>
</template>
<script>
  export default{
    data() {
      return {
        title: 'My app'
      };
    },
    methods: {
      alert() {
        alert('This is an Onsen UI alert notification test.');
      }
    }
  };
</script>
