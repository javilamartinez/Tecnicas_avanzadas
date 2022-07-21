<template>
<v-app>
    <v-row class="mt-5">
    <v-col>
 
      <v-row justify="center">
        <div class="title_proyect">
          <h2>RESPONSABLES DEL PROYECTO</h2>
        </div>
      </v-row>

      <v-row class="box-card" justify="center" >
        <div class="michael" />
        <div class="descripcion">
          <div class="nombredetitulo">
            <h3>Jesús David Ávila Martínez</h3>
          </div>
          <div class="nombredelparrafo">
            <p>Programador/Investigador/Diseñador<br>
              </p>
          </div>
        </div>
      </v-row>
    </v-col>

    <v-col>
   
      <v-row justify="center">
        <div class="title_proyect">
          <h2>UNIVERSIDAD DE CORDOBA</h2>
        </div>
      </v-row>
      <v-row class="box-card" justify="center">
        <div class="logo" />
      </v-row>


   
      <v-row justify="center">
        <div class="title_proyect">
          <h2>DOCENTE</h2>
        </div>
      </v-row>
        <v-row class="box-card" justify="center">
        <div class="aly" />
        <div class="descripcion">
          <div class="nombredetitulo">
            <h3>ALY BENHUR CULCHAC DE LA VEGA</h3>
          </div>
          <div class="nombredelparrafo">
            <p>En Tecnicas Avanzadas de Programación</p>
          </div>
        </div>
      </v-row>

    </v-col>
    </v-row>
    </v-app>
</template>


<style>
.title_proyect{
    color: rgb(255, 255, 255);
}
.box-card {
  margin: 10px 0px 5px 0px;
}
.descripcion {
  padding-left: 60px;
  margin-left: -50px;
  width: 400px;
  height: 50px;
}
.nombredetitulo {
  border-radius: 10px 10px 0px 0px;
  padding-left: 60px;
  margin-left: -50px;
  background-color: rgba(0, 0, 0, 0.3);
  color: rgb(255, 255, 255);
}
.nombredelparrafo {
  border-radius: 10px 0px 0px 0px;
  padding-left: 60px;
  margin-left: -50px;
  height: 100%;
  background-color: rgba(172, 9, 158, 0.9);
  color: rgb(255, 255, 255);
}
.michael {
  border-radius: 90%;
background-image: url(../assets/Team/Jesus_Avila.jpg);
  background-size: cover;
  width: 80px;
  height: 80px;
  position: relative;
  z-index: 2;
}


.usuario5 {
  border-radius: 100%;
  background-image: url();
  background-size: cover;
  width: 80px;
  height: 80px;
  position: relative;
  z-index: 2;
}
.aly {
    border-radius: 100%;
    background-image: url(../assets/Team/Aly.jpeg);
     background-size: cover;   
     width: 90px;
     height: 90px;
     position: relative;
     z-index: 2;
}
</style>
<script>
export default {
  name: "creditos",
  data: () => ({
    //
  }),
  beforeDestroy() {
    },
};
</script>