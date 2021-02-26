C:\laragon\www\portefolio\projet\src
<template>
  <v-app>
    <header>
      <nav>
        <ul>
          <li id="nom-header">
                  <span>
                    MARCEL Evan
                  </span>
          </li>
          <li>
            <a id="a"
               href="#two">
              COMPÉTENCES
            </a>
          </li>
          <li>
            <a id="a"
               href="#three">
              RÉALISATIONS
            </a>
          </li>
          <li>
            <a id="a"
               href="#four">
              STAGE
            </a>
          </li>
          <li>
            <a id="a"
               href="#five">
              CONTACT
            </a>
          </li>
        </ul>
      </nav>
    </header>
    <!--Div page complète-->
    <div class="contenaire">

      <div class="blockHorizontal">

        <!--Slide 1-->
        <div id="one" class="slide one">


          <v-btn v-on:click="salut" style="color: white; background:#0e1012 ">
            On click
          </v-btn>

        </div>

        <!--Slide 2-->
        <div id="two" class="slide two">

          <div class="web text-competence">
            <h2>
              Technologies web :
            </h2>
            <img :src="imgPhp">
            <span>

            </span>
            <img :src="imageTechnoWeb">
            <span>

            </span>
            <img :src="imageSymfony">
            <span>

            </span>
            <img :src="imageVue">
            <span>

            </span>
          </div>
          <v-divider style="width: 80%; margin-right: auto; margin-top: 30px; margin-left: auto"></v-divider>
          <div class="poo text-competence">
            <h2>
              Client lourd :
            </h2>

            <img :src="imageCsharp">
            <span>
            C#
            </span>
            <img :src="imageJava">
            <span>

            </span>

          </div>
          <v-divider style="width: 80%; margin-right: auto; margin-top: 30px; margin-left: auto"></v-divider>
          <div class="autre text-competence">
            <h2>
              Autre :
            </h2>
            <img :src="imageGit">
            <img :src="imageOffice">
            <img :src="imageSql">

          </div>

        </div>

        <!--Slide 3-->
        <div id="three" class="slide three">
          3
        </div>

        <!--Slide 4-->
        <div id="four" class="slide four" tile>
          <!--Stage Com & Company -->
          <v-card width="25%" height="300px" style="border: #0e1012 2px solid">
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
              <v-spacer></v-spacer>
              <v-btn @click="openModalComCompanyVar = true"
                     outlined
                     text
                     style="background-color: #0e1012; color: white; margin-top: -30px;">

                Voir plus
              </v-btn>
            </v-card-actions>
          </v-card>

          <!--Dialog info Stage Com & Company-->
          <v-dialog v-model="openModalComCompanyVar"
                    fullscreen
                    transition="dialog-bottom-transition">
            <v-card height="2000px" width="100%">
              <div class="header-stage">
                <h1 class="text-header-stage">Stage chez Com & Company</h1>
                <v-btn @click="openModalComCompanyVar = false"
                       style="background-color: white; color: #0e1012; float: right" elevation="0" outlined>
                  Fermer
                </v-btn>
              </div>
              <div class="body-stage">
                <h2 class="sous-titre">
                  I - Le groupe :
                </h2>
                <h3 class="sous-sous-titre">
                  1.1 - Valeur et Capital
                </h3>
                <p>
                  Le groupe Valeur et capital est un vaste groupe du domaine de
                  l’immobilier, allant de la location de résidence étudiante à la vente de bien en
                  passant par le conseil en placement financier, ce groupe regroupe de
                  nombreux domaines d’activités ainsi que de nombreux corps de métiers. C’est
                  dans cette démarche qu’il fallut mettre en place une entreprise tierce chargée
                  de s’occuper de la partie numérique de ces différentes entités. C’est alors que
                  Com & Company fut créé.
                </p>
                <h3 class="sous-sous-titre">
                  1.2 - Com & Company
                </h3>
                <p>
                  L’entreprise Com & Company s’occupe de la communication du groupe
                  mais est aussi chargée de créer les différents sites web et autres applications
                  dont nécessitent les nombreuses entités du groupe. La clientèle de Com &
                  Company est donc essentiellement le groupe Valeur et capital. Une nouvelle
                  branche a toutefois vu le jour récemment et celle-ci s’occupe de vendre des
                  prestations informatiques (site web, application) à des entreprises externes au
                  groupe Valeur et capital.
                  Com & Company est une petite entreprise, son pôle développement
                  informatique regroupe une trentaine de salariés mais cela varie en fonction
                  des arrivés et des départs. Elle est située à Lyon à la cité internationale.
                  L’entreprise est une SAS et son chiffre d’affaires en 2018 était de 1 499
                  600 €.
                  Parmi les fonctions principales de Com & Company on retrouve donc la
                  conception et la mise en place de diverses applications comme énoncé plus
                  tôt mais ils assurent aussi bien entendu la maintenance et les mises à jour de
                  leurs applications.
                </p>
                <v-divider style="margin-top: 30px">
                </v-divider>
                <h2 class="sous-titre">
                  II - Les technologies utilisés :
                </h2>
                <div class="block-techno">
                  <div class="div-image-techno">
                    <img :src="imageVue">
                  </div>
                  <div class="div-image-techno">
                    <img :src="imageSymfony">
                  </div>

                </div>
                <v-divider style="margin-top: 30px"></v-divider>
                <h2 class="sous-titre">
                  III - Ma mission :
                </h2>
                <h3 class="sous-sous-titre">
                  3.1 - Contexte de la mission
                </h3>
                <p>
                  Parmi les différents projets de l’entreprise j’ai été assigné à un site de
                  signature à distance, en effet à cause du confinement les signatures de
                  documents en présentiel n’étaient plus possible c’est pour répondre à cette
                  problématique que le site « Sign » a dû être mis en place. Cette plateforme
                  permet donc d’accéder aux différentes entités de l’entreprise et de pouvoir
                  émettre des signatures facilement et ergonomiquement.
                </p>

                <h3 class="sous-sous-titre">
                  3.2 - Le cœur de la mission
                </h3>
                <p>
                  Ma mission à été en partant du site Sign de créer de nouvelles
                  fonctionnalités utiles à l’administration des utilisateurs.
                  Le projet est développé en PHP avec le Framework Symfony pour le back
                  mais aussi avec un Framework javascript pour le front, nommé vuejs.
                  Les problématiques principales ont été d’arriver sur un projet déjà
                  existant et de se familiariser avec celui-ci, notamment pour comprendre
                  comment étaient géré certaines fonctionnalités mais aussi pour intégrer les
                  problématiques métiers inerrant au site. La deuxième problématique à été de
                  se familiariser avec les différents Framework qui composent le site. Pour moi la
                  compréhension du Symfony a été compliqué, n’ayant jamais fait de PHP objet
                  j’ai au début été vraiment pris au dépourvut, mais après beaucoup de
                  persévérance j’ai appris à être de plus en plus à l’aise avec ce Framework et je
                  suis désormais capable de bien le comprendre.
                </p>

              </div>
            </v-card>

          </v-dialog>


        </div>
      </div>
    </div>
  </v-app>
</template>


<script>


export default {

  icons: {
    iconfont: 'mdiSVG'
  },
  name: 'App',

  data: () => ({
    name: 'Evan',
    openModalComCompanyVar: false,
    imageCEC: require('@/img/com-&-company.webp'),
    imageVue: require('@/img/vuejs.png'),
    imageSymfony: require('@/img/symfony.png'),
    imgPhp: require('@/img/new-php-logo.svg'),
    imageCsharp: require('@/img/logo-csharp.png'),
    imageJava: require('@/img/logo-java-mieux.jpg'),
    imageTechnoWeb: require('@/img/html-css.png'),
    imageGit: require('@/img/logo-github.png'),
    imageOffice: require('@/img/logo-office.png'),
    imageSql: require('@/img/logo-sql.png')

  }),
  methods: {
    salut: function () {
      alert("Bonjour" + " " + this.name + " !")
    },
    test: function () {
      window.scrollY
    }
  },
};
</script>

<style>
*, ::after, ::before {
  margin: 0;
  padding: 0;


}

header {
  position: fixed;
  width: 100vw;
  background-color: #0e1012;
  padding: 30px;
  z-index: 99;
}


.contenaire {
  width: 500vh;
  height: 100vw;
  transform: rotate(-90deg) translateX(-100vh);
  transform-origin: top left;
  overflow-x: hidden;
  -ms-overlow-style: none;
  scrollbar-width: none;
  position: relative;
}

::-webkit-scrollbar {
  display: none;
}

.blockHorizontal {
  display: flex;
  flex-direction: row;
  width: 400vw;
  height: 100vh;
  transform: rotate(90deg) translateY(-100vh);
  transform-origin: top left;
}


.slide {
  width: 100vw;
  height: 100vh;
  justify-content: center;
  align-items: center;
  border: #0e1012 1px solid;

}

.one {
  background: white;
  display: flex;
}

.two {
  background: white;

}

.three {
  background: white;
  display: flex;
}

.four {
  background: white;
  display: flex;
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
  padding-bottom: 7px;
  color: white;

}


nav li span {

  font-size: 40px;
  color: white;
}

.web {
  margin-top: 11%;
  display: flex;
  height: 20%;
  justify-content: center;
  align-items: center;
}

.text-competence h2 {
  text-align: center;
  font-size: 30px;
  margin: 40px;
}

.poo {
  display: flex;
  height: 20%;
  justify-content: center;
  align-items: center;
}


.autre {
  height: 20%;
  margin-top: 0px;
  display: flex;
  justify-content: center;
  align-items: center;
}


.text-competence span {
  display: block;
  float: bottom;
}


.two img {
  height: 50px;
  width: 50px;
  margin: 40px;
}

.header-stage {
  width: 100%;
  height: 100px;
  background-color: #0e1012;
  display: flex;
  text-align: center;
  position: sticky;
  top: 0;


}

.text-header-stage {
  color: white;
  margin: auto;
  font-size: 50px;
}

.body-stage {
  width: 50%;
  margin: auto;
  height: auto;
}

.block-techno {
  height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.div-image-techno {
  height: 150px;
  width: 150px;
  margin: 130px;
}

p {
  margin-top: 10px;
}


.sous-titre {
  margin-top: 30px;
  text-align: center;
}

.sous-sous-titre {
  margin-top: 30px;
}
</style>
