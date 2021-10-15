<template>
  <div class="hello">
    <h1>{{ msg }}</h1>

    <div class="container">
      <b-carousel
        id="carousel-1"
        v-model="slide"
        :interval="4000"
        controls
        indicators
        background="#ababab"
        img-width="1024"
        img-height="400"
        style="text-shadow: 1px 1px 2px #333"
        @sliding-start="onSlideStart"
        @sliding-end="onSlideEnd"
      >
        <!-- Text slides with image -->
        <b-carousel-slide
          img-src="https://image.shutterstock.com/image-photo/behind-football-goalposts-during-amateur-600w-394746547.jpg"
        >
          <h1>Variedad en campos de juego</h1>
        </b-carousel-slide>

        <!-- Slides with custom text -->
        <b-carousel-slide
          img-src="https://image.shutterstock.com/image-photo/soccer-field-view-corner-children-600w-613283609.jpg"
        >
          <h1>Comparte en familia</h1>
        </b-carousel-slide>

        <!-- Slides with image only -->
        <b-carousel-slide
          img-src="https://image.shutterstock.com/image-photo/rickmansworth-hertfordshire-uk-september-20th-600w-1184296489.jpg"
        >
          <h1>Disfruta con amigos</h1>
        </b-carousel-slide>

        <!-- Slides with img slot -->
        <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
        <b-carousel-slide>
          <template #img>
            <img
              class="d-block img-fluid w-100"
              width="1024"
              height="400"
              src="https://image.shutterstock.com/image-photo/soccer-players-middle-artificial-pitch-600w-771973045.jpg"
              alt="image slot"
            />
          </template>
        </b-carousel-slide>
      </b-carousel>

      <p class="mt-4">
        Slide #: {{ slide }}<br />
        <br />
        <!-- Sliding: {{ sliding }} -->
      </p>
      
    </div>
    <div class="h2 mb-0">
      <h2 class="font_1" style="font-size:45px">
        <span style="color:#3B805A">
          <span style="font-size:45px">
            <font face="Bahnschrift">Canchas recomendadas en Bogotá</font>
          </span>
        </span>
      </h2>
    </div>
    <div>
      <span>
        <font face="Bahnschrift">
          <p style="border: ridge #0f0fef 1px;">
            Aquí encontrarás el listado de LAS MEJORES CANCHAS DE FÚTBOL
          </p>
        </font>
      </span>  
    </div>
    <!-- <div class="row">
      <div id="container" class="column mx-5" align="left">
          <b-img src="https://image.shutterstock.com/image-photo/soccer-players-middle-artificial-pitch-600w-771973045.jpg" fluid alt="Fluid image"></b-img>
          <span class="font_2" style="font-size:45px">Cancha:</span>
          <span>
            <router-link  router-link to="/notas" class="reg mx-2">Regístrate</router-link>
          </span>
      </div>
      <div class="column">
        <span class="font_2" style="font-size:45px">Cancha:</span>
      </div>
    </div> -->

    <div class="row">
      <div class="column">
        <b-img src="https://image.shutterstock.com/image-photo/soccer-players-middle-artificial-pitch-600w-771973045.jpg" fluid alt="Fluid image"></b-img>
      </div>
      <div class="column" align="left">
        <br />
        <span class="font_2" style="font-size:45px">
          <span style="color:#3B805A">
            Cancha: 
          </span>
        </span>
        <span class="font_2" style="font-size:45px">
          <span style="color:#14638c">
            Zona Centro
          </span>
        </span>
      <div>
        <span class="font_2" style="font-size:45px">
          <span style="color:#010101">
            Ciudad: 
          </span>
        </span>
        <span class="font_2" style="font-size:45px">
          <span style="color:#14638c">
            Bogotá
          </span>
        </span>
      </div>
      <div>
        <span class="font_2" style="font-size:45px">
          <span style="color:#010101">
            Dirección: 
          </span>
        </span>
        <span class="font_2" style="font-size:45px">
          <span style="color:#14638c">
            Calle 19 # 11 - 71
          </span>
        </span>
      </div>
      <div>
        <span class="font_2" style="font-size:45px">
          <span style="color:#010101">
            Teléfono: 
          </span>
        </span>
        <span class="font_2" style="font-size:45px">
          <span style="color:#14638c">
            5-55-5555
          </span>
        </span>
      </div>
        <span style="font-size:45px">
          <router-link  router-link to="/notas">Regístrate</router-link>
        </span>
      </div>
    </div>



  </div>
</template>
    <!-- <p>
      For a guide and recipes on how to configure / customize this project,<br />
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener"
        >vue-cli documentation</a
      >.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel"
          target="_blank"
          rel="noopener"
          >babel</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-router"
          target="_blank"
          rel="noopener"
          >router</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-vuex"
          target="_blank"
          rel="noopener"
          >vuex</a
        >
      </li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li>
        <a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a>
      </li>
      <li>
        <a href="https://forum.vuejs.org" target="_blank" rel="noopener"
          >Forum</a
        >
      </li>
      <li>
        <a href="https://chat.vuejs.org" target="_blank" rel="noopener"
          >Community Chat</a
        >
      </li>
      <li>
        <a href="https://twitter.com/vuejs" target="_blank" rel="noopener"
          >Twitter</a
        >
      </li>
      <li>
        <a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a>
      </li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li>
        <a href="https://router.vuejs.org" target="_blank" rel="noopener"
          >vue-router</a
        >
      </li>
      <li>
        <a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-devtools#vue-devtools"
          target="_blank"
          rel="noopener"
          >vue-devtools</a
        >
      </li>
      <li>
        <a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener"
          >vue-loader</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/awesome-vue"
          target="_blank"
          rel="noopener"
          >awesome-vue</a
        >
      </li>
     </ul> -->

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      slide: 0,
      sliding: null,
    };
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true;
    },
    onSlideEnd(slide) {
      this.sliding = false;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}


*{
  box-sizing: border-box;
}

/* Create two equal columns that floats next to each other */
.column {
  float: left;
  width: 50%;
  padding: 10px;
  height: 300px; /* Should be removed. Only for demonstration */
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

</style>
