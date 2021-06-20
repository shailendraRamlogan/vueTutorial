<template>
  <v-container>
    <v-toolbar flat>
      <v-toolbar-title>PHOTOGRAPHY</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items class="hidden-xs-only">
        <v-btn text to="/">
          HOME  
        </v-btn>
        <v-btn text to="/about">
          ABOUT
        </v-btn>
        <v-btn text to="/contact">
          CONTACT
        </v-btn>
      </v-toolbar-items>
      <div class="hidden-sm-and-up">
        <v-menu offset-y>
        <template v-slot:activator="{ on }">
            <v-app-bar-nav-icon v-on="on"></v-app-bar-nav-icon>
        </template>
        <v-list class="responsiveMenu">
          <v-list-item>
            <v-list-item-title><router-link to="/">HOME</router-link></v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title><router-link to="/about">ABOUT</router-link></v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title><router-link to="/contact">CONTACT</router-link></v-list-item-title>
          </v-list-item>
        </v-list>
    </v-menu>
      </div>
    </v-toolbar>
  </v-container>
</template>

<script>
  export default {
    name: 'Header',

    data: () => ({
    }),
  }
</script>
