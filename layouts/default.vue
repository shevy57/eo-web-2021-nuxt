<template>
  <v-app light>
   <topbar/>
   <nuxt/>
   <footersection/>
  </v-app>
</template>

<script>
export default {
  
  data() {
    return {
      
    
    }
  },
}
</script>
<style >
.theme--light.v-application {
    background: #dbdbdb !important;
    color: rgba(0, 0, 0, 0.87);
}
body{
   font-family: "Roboto Slab", "Times New Roman", serif;
}
</style>