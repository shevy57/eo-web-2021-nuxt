<template>
  <div>
    <v-app-bar
      color="white accent-4"
      dense
      light
      class="mobile-menu rounded-b-sm"
      elevation="7"
    >
      <v-toolbar-title class="title">Material Kit Nuxt</v-toolbar-title>

      <v-spacer></v-spacer>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" absolute>
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item class="border-light pa-2">
            <v-list-item-title>
              <v-menu offset-y class="me-0">
                <template v-slot:activator="{ on, attrs }">
                  <v-btn
                    class="bg-transparent  text-dark"
                    elevation="0"
                    v-bind="attrs"
                    v-on="on"
                  >
                    Dropdown
                    <v-icon>mdi-menu-down</v-icon>
                  </v-btn>
                </template>
                <v-list>
                  <v-list-item v-for="(item, index) in items" :key="index">
                    <v-list-item-title>{{ item.title }}</v-list-item-title>
                  </v-list-item>
                </v-list>
              </v-menu></v-list-item-title
            >
          </v-list-item>

          <v-list-item class="border-light pa-2">
            <v-list-item-title>
              <v-btn class="bg-transparent " elevation="0">
                <v-icon class="mr-1 text-dark">mdi-printer</v-icon>
                Upgrade to pro
              </v-btn></v-list-item-title
            >
          </v-list-item>

          <v-list-item class="border-light pa-2">
            <v-list-item-title
              ><v-btn class="bg-transparent text-dark" elevation="0">
                <v-icon class="mr-1">mdi-cloud-download</v-icon>
                download
              </v-btn></v-list-item-title
            >
          </v-list-item>

          <v-list-item class="border-light pa-2">
            <v-list-item-title>
              <nuxt-link to="sampe" icon class="text-decoration-none pl-4">
                <v-icon class="text-dark">mdi-twitter</v-icon>
              </nuxt-link></v-list-item-title
            >
          </v-list-item>
          
          <v-list-item class="border-light pa-2">
            <v-list-item-title>
              <nuxt-link to="sampe" icon class="text-decoration-none pl-4">
                <v-icon class="text-dark">mdi-facebook</v-icon>
              </nuxt-link></v-list-item-title
            >
          </v-list-item>
          
          <v-list-item class="border-light pa-2">
            <v-list-item-title>
              <nuxt-link to="sampe" icon class="text-decoration-none pl-4">
                <v-icon class="text-dark">mdi-instagram</v-icon>
              </nuxt-link></v-list-item-title
            >
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>
<script>
export default {
  data() {
    return {
      drawer: false,
      group: null,
      items: [
        { title: 'All Components' },
        { title: 'Documentation' }
     
      ],
    }
  },
  watch: {
    group() {
      this.drawer = false
    },
  },
}
</script>

<style scoped>
.mobile-menu {
  height: 68px !important;
  margin-top: 0px;
  transform: translateY(0px);
  left: 0px;
  right: 0px;
  padding: 10px 4px;
  position: fixed;
  z-index: 5;
}
.title {
  font-size: 18px !important;
  font-family: 'Roboto', 'Helvetica', 'Arial', sans-serif;
  font-weight: 300;
  line-height: 30px;
}
.v-navigation-drawer--absolute {
  position: absolute;
  z-index: 99;
  padding-top: 50px;
}
.theme--light.v-btn.v-btn--has-bg {
  background-color: transparent;
  font-size: 12px;
  font-size: 12px;
  font-weight: 400;
  line-height: 20px;
}
.text-dark {
    color: #424242 !important;
}
.theme--light.v-list-item:not(.v-list-item--active):not(.v-list-item--disabled) {
    
    border-radius: 0px;
    
}
.v-navigation-drawer .v-list:not(.v-select-list) {
    background: inherit;
    padding: 0px 2px !important;
}
.border-light{
    color: #424242 !important;
}
.v-navigation-drawer .v-icon.v-icon{
    font-size: 20px !important;
}
</style>