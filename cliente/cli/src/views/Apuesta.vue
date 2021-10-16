<template>
  <div class="apuesta">
    <body>  
    </body>
    <h1>Proximamente Disponible!</h1>
    <br /><br /><br /><br /><br />
    <div>
      <span class="font_2" style="font-size: 45px">
        <span style="color: #3b805a">
          <font face="Bahnschrift"> Nuestros colaboradores </font>
        </span>
      </span>
    </div>
    <br /><br /><br />

    <div class="row">
      <div class="columna">
        <img src="../assets/img02.jpg" height="295">
      </div>
      <div class="columna">
        <img src="../assets/img01.jpg" height="295">
      </div>
      <div class="columna">
        <img src="../assets/img03.jpg" height="295">
        <br /><br />
      </div>
    </div>
    <div class="row">
      <div class="columna">
        <span style="color:#010101">
          <font face="Bernard MT Condensed">Wilder Hernández Castro</font>
        </span>
      </div>
      <div class="columna">
        <span style="color:#010101">
          <font face="Bernard MT Condensed">Luis Alberto Ramírez</font>
        </span>
      </div>
      <div class="columna">
        <span style="color:#010101">
          <font face="Bernard MT Condensed">Jefferson Guzmán Preciado</font>
        </span>
      </div>
    </div>
  </div>
</template>


<style scoped>

.columna {
  float: left;
  width: 33%;
  border: 0px solid;
}
@media (max-width: 980px) {
  .columna {
    float: none;
    width: 100%;
  }
}

body{
  background-image: url("../assets/background.jpg");
}

</style>
