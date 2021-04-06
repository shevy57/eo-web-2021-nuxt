<template>
<div >
  <div class="web-topbar">
      <v-toolbar dense elevation="0" class="position-fixed header-transparent" id="header">
    <v-toolbar-title class="mr-auto toolbartitle font-weight-light" id=""
      >Materail Kit Nuxt</v-toolbar-title
    >

    <v-spacer></v-spacer>

    <v-menu offset-y class="me-0">
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          class="bg-transparent v-btn"
          elevation="0"
          v-bind="attrs"
          v-on="on"
          
        >
          Dropdown
          <v-icon>mdi-menu-down</v-icon>
        </v-btn>
      </template>
      <v-list dense class="pa-2">
        <nuxt-link to="sample" class="text-decoration-none hover">
<v-list-item v-for="(item, index) in items" :key="index" class="tile">
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
        </nuxt-link>
        
      </v-list>
    </v-menu>

    <v-btn class="bg-transparent v-btn" elevation="0">
      <v-icon class="mr-1">mdi-printer</v-icon>
      Upgrade to pro
    </v-btn>

    <v-btn class="bg-transparent v-btn" elevation="0">
      <v-icon class="mr-1">mdi-cloud-download</v-icon>
      download
    </v-btn>
    <v-tooltip bottom>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          class="bg-transparent v-btn"
          elevation="0"
          v-bind="attrs"
          v-on="on"
        >
          <v-icon class="">mdi-twitter</v-icon>
        </v-btn>
      </template>
      <span >Follow us on twitter</span>
    </v-tooltip>
    <v-tooltip bottom>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          class="bg-transparent v-btn"
          elevation="0"
          v-bind="attrs"
          v-on="on"
        >
          <v-icon class="">mdi-facebook</v-icon>
        </v-btn>
      </template>
      <span>Follow us on facebook</span>
    </v-tooltip>
    <v-tooltip bottom>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          class="bg-transparent v-btn"
          elevation="0"
          v-bind="attrs"
          v-on="on"
        >
          <v-icon class="">mdi-instagram</v-icon>
        </v-btn>
      </template>
      <span>Follow us on instagram</span>
    </v-tooltip>
  </v-toolbar>
  </div>
  <div class="mobile-topbar " relative>
    <mobilemenu/>
  </div>
</div>

  
</template>

<script>

export default {
  
  data() {
    return {
      items: [
       { title: 'All Components' },
        { title: 'Documentation' }
      ],
    }
  },
  mounted() {
    window.onscroll = function () {
      scrollFunction()
    }

    function scrollFunction() {
      if (
        document.body.scrollTop > 400 ||
        document.documentElement.scrollTop > 400
      ) {
        document.getElementById('header').style.background = 'white'
       var x=  document.getElementById('header')
       x.classList.add("header-white")
        x.classList.remove("header-transparent")

      } else {
        document.getElementById('header').style.background = 'transparent'
       var x=  document.getElementById('header')
       x.classList.add("header-transparent")
        x.classList.remove("header-white")
      }
    }
  },
}
</script>
<style scoped>
#header {
  background: transparent;
  z-index: 5;
}
.bg-transparent {
  background-color: transparent !important;
}
.position-fixed {
  position: fixed;
  z-index: 2;
}
.v-sheet.v-toolbar:not(.v-sheet--outlined) {
  width: 100%;
  padding: 28px 120px;
  height: auto !important;
}
.v-btn:not(.v-btn--round).v-size--default {
  height: 36px;
  min-width: 64px;
  padding: 25px 13px !important;
  font-size: 12px;
  color: white;
}
.v-toolbar__title {
  color: white;
}
.header-transparent .v-btn, .header-transparent .toolbartitle{
  color: white !important;
}
.header-white .v-btn, .header-white .toolbartitle{
  color: #3c4858 !important;
  
}
.mobile-topbar{
    display: none;
  }
@media(max-width:960px){
  .mobile-topbar{
    display: block;
    
  }
  .web-topbar{
    display: none;
  }
}
.theme--light.v-list-item:not(.v-list-item--active):not(.v-list-item--disabled) {
    color: rgba(0, 0, 0, 0.87) !important;
    
} 
.theme--light.v-list-item:not(.v-list-item--active):not(.v-list-item--disabled):hover {
    color: white !important;
    background-color: #9c27b0;
}
</style>