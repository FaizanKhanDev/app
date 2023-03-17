<template>
    <v-app-bar app>
      <div class="links d-flex">
        <div v-for="item in items" :key="item.id">
          <nuxt-link :to="item.url" class="text-decoration-none white--text">{{ item.title }}</nuxt-link>
        </div>

      </div>
      <v-spacer></v-spacer>
      <v-btn class="dowloadCv">Dowload My Cv</v-btn>
    </v-app-bar>
  </template>
  
  <script>
  export default {
    name: "Appbar",
    data() {
      return {
        items: [
          {
            url: "/",
            title: "Home",
          },
          {
            url: "/about",
            title: "About",
          },
          {
            url: "/services",
            title: "Services",
          },
          {
            url: "/contacts",
            title: "Contacts",
          },
        ],
      };
    },
  };
  </script>
  
  <style>
  
  .links {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-right: 50px;
  }
  
  .links div {
    margin-right: 45px;
    margin-left: 30px;
  }

  </style>
  