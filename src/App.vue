<template>
  <v-app>
    <!--Div page complète-->
    <div class="contenaire">
      <div class="blockHorizontal">
        <header>
          <nav>
            <ul>
              <li id="nom-header">
            <span id="lettre-m">
              M
            </span>
                <span>
              ARCEL
            </span>
                <span id="lettre-e">
              E
            </span>

                <span>
              VAN
            </span>

              </li>
              <li>
                <a id="a">
                  COMPÉTENCES
                </a>
              </li>
              <li>
                <a id="a"
                   href="#slide">
                  FORMATIONS
                </a>
              </li>
              <li>
                <a id="a">
                  STAGE
                </a>
              </li>
              <li>
                <a id="a">

                  RÉALISATIONS
                </a>
              </li>
              <li>
                <a id="a">
                  CONTACT
                </a>
              </li>
            </ul>
          </nav>
        </header>
        <!--Slide 1-->
        <div class="slide one">


          <v-btn v-on:click="salut" style="color: white; background:#0e1012 ">
            On click
          </v-btn>

        </div>

        <!--Slide 2-->
        <div class="slide two">
          2
        </div>

        <!--Slide 3-->
        <div class="slide three">
          3
        </div>

        <!--Slide 4-->
        <div class="slide four" tile>
          <!--Stage Com & Company -->
          <v-card width="25%" height="300px" style="border:1px solid black">
            <v-card-title class="text-center">
              Com & Company
            </v-card-title>
            <v-divider style="margin-top: -15px; width: 75%; margin-left: auto; margin-right: auto"></v-divider>
            <v-card-text>
              Stage dans l'entreprise Com & Company. Cette entreprise est une SSII appartenant au groupe valeur et
              capital
            </v-card-text>
            <img
                :src="imageCEC"
                style="margin-top: -50px; margin-left: auto; margin-right: auto; padding: 0; display: block">
            <v-card-actions>

              <v-btn @click="openModalComCompanyVar = true"
                     outlined
                     text
                     style="background-color: #0e1012; color: white; margin-top: -30px">

                Voir plus
              </v-btn>
            </v-card-actions>
          </v-card>
          <v-dialog v-model="openModalComCompanyVar"
                    fullscreen
                    transition="dialog-bottom-transition">

            <v-card height="100vh" width="100vw">


              <v-btn @click="openModalComCompanyVar = false">
                Fermer
              </v-btn>
            </v-card>

          </v-dialog>
        </div>

      </div>

    </div>

  </v-app>
</template>

<script>


export default {
  name: 'App',

  data: () => ({
    name: 'Evan',
    openModalComCompanyVar: false,
    imageCEC: require('@/img/com-&-company.webp'),

  }),
  methods: {
    salut: function () {
      alert("Bonjour" + " " + this.name + " !")
    },
  },
};
</script>

<style>

.contenaire {
  width: 100vh;
  height: 100vw;
  transform: rotate(-90deg) translateX(-100vh);
  transform-origin: top left;
  overflow-x: hidden;
  -ms-overlow-style: none;
  scrollbar-width: none;

}

::-webkit-scrollbar {
  display: none;
}

.blockHorizontal {
  display: flex;
  flex-direction: row;
  width: 400vw;
  transform: rotate(90deg) translateY(-100vh);
  transform-origin: top left;
}


.slide {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 100px;
  border: #0e1012 1px solid;
}

.one {
  background: white;
}

.two {
  background: white;
}

.three {
  background: white;
}

.four {
  background: white;
}


header {
  background-color: #0e1012;
  width: 100vw;
  top: 0;
  left: 0;
  position: fixed;
  height: 100px;
  padding: 0;


}

nav {
  padding: 0;
  text-align: center;
}

nav li {
  display: inline;
  list-style: none;
  font-size: 15px;
  padding: 30px;

}

/* Les id "a" correspondent à plusieurs élément car le code css ci-dessous ne fonctionne pas en appelant l'élément ou en utilisant une class */

#a {
  color: white;
  text-decoration: inherit;
  transition-property: padding-bottom;
  transition-duration: 0.5s;
  padding-bottom: 0px;
}

#a:hover {
  border-bottom: white solid 3px;
  padding-bottom: 15px;
  color: white;

}


nav li span {

  font-size: 40px;
  color: white;
}


</style>
