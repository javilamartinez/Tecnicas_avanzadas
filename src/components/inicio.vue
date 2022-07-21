<template>
  <v-app>
    
    

    <v-main>
      <div class="img">
        <v-img
      src="../assets/Background/001.png"
      max-width="1000"
 
    >
        </v-img>
      </div>
<div class="icon">
      <router-link to="/entrada">
     <v-btn
        class="ma-0"
        color="red"
        dark
      >
          LETS GO
        <v-icon
          dark
          right
        >
        mdi-arrow-up-bold-box-outline
        </v-icon>
      </v-btn>
            </router-link>
            </div>
         
  
            
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'inicio', 
  components: {
    
  },
  data: () => {
  
    return {
          
    
    };
  }
};
</script>

<style>
#app {
  background: url('../assets/Background/01.gif') no-repeat center center fixed !important;
  background-size: cover;
  position: relative;
  overflow-x:hidden; 
  overflow-y:hidden;
} 
.title {
color:  rgb(255, 255, 255);
text-align: right;
position: relative;
  bottom: -200px;
   right: 200px;
}
.subtitle {
  color:  white;
text-align: right;
position: relative;
  bottom: -220px;
   right: 170px;
   font-size: 35px;
  
}
body{
  margin: 0; 
  padding: 0;
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

.icon {
     padding-top: 540px;
     left:-50px
}
.img{
  text-align: right;
position: relative;
  bottom: -11px;
   right: -160px;
   font-size: 35px;
  
}
</style>