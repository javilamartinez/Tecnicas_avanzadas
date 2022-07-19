<template>
<div id="principal">
     <!-- <v-sheet elevation="8">
<v-tabs
      background-color="red"
      dark
      show-arrows
    >
      <v-tabs-slider color="yellow"></v-tabs-slider>
      <v-tab :to="{ name: 'contenido' }" class="font-italic">Contenido
          <v-icon   x-small class="mb-5"></v-icon>
          </v-tab>

          <v-tab :to="{ name: 'actividades' }" class="font-italic">Actividades
          </v-tab>

        <v-tab :to="{ name: 'evaluacion' }" class="font-italic">Evaluación
            <v-icon x-large class="mb-5">fas fa-clipboard-check</v-icon>
          </v-tab>
          
          <v-tab :to="{ name: 'creditos' }" class="font-italic">Creditos
            <v-icon x-large class="mb-5">fas fa-clipboard-check</v-icon>
          </v-tab>
          
    </v-tabs>
 
  </v-sheet>-->
    
  <v-card>
    <v-tabs
      v-model="tab"
      background-color="deep-purple accent-4"
      centered
      dark
      icons-and-text
    >
      <v-tabs-slider></v-tabs-slider>

      <v-tab :to="{ name: 'contenido' }" href="#tab-1">
        <v-icon>Contenido</v-icon>
      </v-tab>

      <v-tab :to="{ name: 'actividades' }" href="#tab-2">
        <v-icon>Actividades</v-icon>
      </v-tab>

      <v-tab :to="{ name: 'evaluacion' }" href="#tab-3">
        <v-icon>Evaluación</v-icon>
      </v-tab>
       <v-tab :to="{ name: 'creditos' }" href="#tab-4">
        <v-icon>Creditos</v-icon>
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="i in 3"
        :key="i"
        :value="'tab-' + i"
      >
        <v-card flat>
          <v-card-text>{{ text }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>


 <!-- <v-img
      src="../assets/Ilustraciones/03.png"
      max-width="600"
     >
 </v-img>
      <div class="icon">
         <v-img
      src="../assets/Ilustraciones/02.png"
     max-width="800"
  >
           </v-img>
           -->
 
 
 <v-main>
      <transition name="bounce">
        <router-view> 
      

                  </router-view>
      </transition>
    </v-main>

 </div>
  
  

</template>

<script>
export default {
  name: 'Entrada', 
  components: {
    
  },
  data: () => {
  
    return {
          
    
    };
  }
};
</script>

<style>
#principal {
 background: url('../assets/Background/2.jpg') no-repeat center center fixed !important;
  
}
.title {
color:  white;
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
    align-content: right;
    align-items: right;
    padding-left: 50%;
    position: relative;
  bottom: 450px;
   right: -60px;
   font-size: 50px;
    
}
</style>