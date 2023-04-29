<template>
  <v-app>
   
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
      
      color="black"
      height="80"
      class="px-16"
    >
      <img src="../static/logo.webp" alt="" width="200" class="ml-16" >
      <v-spacer/>
      
    <v-btn text x-large class="topBar" color="white" to="/about">ABOUT US</v-btn>
        <v-btn text x-large color="white" to="/talent">TALENT</v-btn>
        <v-btn text x-large color="white" to="/refer">REFER</v-btn>

        <v-btn text x-large color="white" to="/blogs">OUR BLOGS</v-btn>
        <v-btn text x-large color="white" to="/franchise">OPEN A FRANCHISE</v-btn>
        <v-btn
      class="mx-2 buttonRotate"
      fab
      dark
      small
      color="primary"
      
    >
      <img src="../static/63c7df7cc446588f6d13ef8b_button_icon_blue.svg" alt="">
    </v-btn>
        <v-btn text x-large color="primary" class="pl-0" to="/">APPLY NOW</v-btn>
     
    </v-app-bar>
    <v-main >
      <v-container fluid class="pa-0">
        <Nuxt />
      </v-container>
    </v-main>
    
    <v-container
    fluid
   style="background-color: black;"
   class="pt-16" >
    <v-card  color="transparent" class="mt-16">
      <div class="text-center">
        <img src="../static/footerLogo.svg" alt="" width="100">
      </div>
      <v-card width="400"  color="transparent" class="secondary--text mt-4 mx-auto">
        Travel the world, Live your best life, Make money and become one of the most loved influencers in the world.
      </v-card>
      <div class="d-flex flex-wrap justify-space-between my-16 px-16">
        <v-btn text x-large color="white">ABOUT US</v-btn>
        <v-btn text x-large color="white">OUR SERVICES</v-btn>
        <v-btn text x-large color="white">TALENT</v-btn>
        <v-btn text x-large color="white">OUR BLOGS</v-btn>
        <v-btn text x-large color="white">OPEN A FRANCHISE</v-btn>
        <v-btn text x-large color="white">CONTACT US</v-btn>
        <v-btn text x-large color="white">PRIVACY POLICY & LEGAL</v-btn>
        <v-btn text x-large color="white">APPLY NOW</v-btn>

      </div>
      <div class="text-center">
        <img src="../static/Outline.svg" alt="" width="30">
        <img src="../static/Vector.svg" alt="" width="30" class="ml-4">
      </div>
      <div class="justify-center d-flex my-16"><h4 class="secondary--text mr-2">&copy; {{ new Date().getFullYear() }}</h4><h4 class="secondary--text">Banx Management. All Rights Reserved</h4></div>
    </v-card>
    </v-container>
   
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
<style>
.topBar.v-btn:focus {
  background: transparent !important;
  color: #fbbf23 !important;
}
.v-btn--fab.v-size--small {
    height: 34px !important;
    width: 34px !important;
}
.v-btn.v-size--x-large {
    font-size: 1.20rem !important;
    font-weight: 600 !important;
}
.buttonRotate:hover {
  transform: rotate(90deg);
}
h1 {
  font-size: 4rem !important;
  font-weight: 700;
  font-family: Montserrat, sans-serif !important;
}
p {
  font-size: 24px !important;
  color: #999999 !important;
  font-family: Inter, sans-serif;
    line-height: 1.7 !important;
}
li {
  font-size: 18px !important;
  color: rgba(23, 26, 26, .6) !important;
  font-family: Inter, sans-serif;
    line-height: 1.7;
    margin-top: 30px;
}
 .v-expansion-panel-header{
  font-size: 1rem !important;

} 
.v-expansion-panel {
  border: 1px solid black;
  border-top-left-radius: 0px !important;
  border-top-right-radius: 0px !important;
  padding: 30px 5px !important;
}
.box {
  margin-top: 160px;
}
.home4 {
  background-image: url("../static/63c80a614588a34b5690563c_home_become_img.webp");
  background-size: contain;
  background-position-x: left;
  
}
.home5 {
  background-image: url("../static/bottom.webp");
  background-position-x: right;
  background-size: 100%, 100%;
}
.containerPadding{
  padding-left: 150px;
}
.bg{
  background-color: red;
}
</style>