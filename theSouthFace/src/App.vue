<script>
import navBarVue from "./components/navBar.vue";
import { RouterLink, RouterView } from "vue-router";

export default{
  name:"App",
  components:{
    navBarVue
  }
}
</script>

<template>
<navBarVue v-if="this.$route.name!=='LandingPage'"/>
  <RouterView />
  <h2 v-if="this.$route.name==='HomePage'">More products coming soon!</h2>
  <h6 class="copyright">All images used in this website belongs to their respectful owner</h6>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500&display=swap');
html {
  font-family: 'poppins', sans-serif;
  height: 100%;
}

body {
  background-image: linear-gradient(rgba(0,0,0,0.8), rgb(0,0,0,0.8)),url(https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/9948bc52-ac5c-4c1f-9fad-711c3b52a82b/mechanical-keyboards-rama.jpg);
  background-size: cover;
  height:100%
}.copyright {
  position:fixed;
  color : white;
  font-size: 10px;
  bottom: 0 ;
  padding-left: 20px;
}
h2{
  color: white;
  text-align: center;
  margin-bottom: 20px;
}
</style>
