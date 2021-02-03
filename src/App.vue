<template>
  <v-app>


      <!--Div page complète-->
      <div class="contenaire">
        <div class="blockHorizontal">

        <!--Slide 1-->
        <div class="slide one">
          <header id="header1">
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
                  <a id="a">
                    FORMATIONS
                  </a>
                </li>
                <li>
                  <a id="a">
                    CURRICULUM VITÆ
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
        </div>

        <!--Slide 2-->
        <div class="slide two">

        </div>

        <!--Slide 3-->
        <v-div class="slide three" >
        3
        </v-div>

        <!--Slide 4-->
        <div class="slide four" tile>
        4
        </div>

        </div>

      </div>

  </v-app>
</template>

<script>


export default {
  name: 'App',

  data: () => ({}),


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


.slide{
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size:100px
}

.one {
  background: white;
}

.two{
  background: aqua;
}

.three {
  background: antiquewhite;
}

.four{
  background: beige;
}




header {
  background-color: black;
  width: 100vw;
  position: fixed;
  top:0;


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

#div-home {
  height: 100%;
  width: 100%;
  background-color: black;

}

#div-home:hover {
  animation-duration: 1s;
  animation-name: transition-oppacite;
  animation-fill-mode: forwards;

}

@keyframes transition-oppacite {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}


nav li span {

  font-size: 40px;
  color: white;
  animation-duration: 3s;
  animation-name: translate-left-nom;
  animation-iteration-count: 1;
  animation: forwards;
}


@keyframes translate-left-nom {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

#div-card-presentation-premier50 {
  width: 50%;
  height: 90%;
  margin: auto;
  float: left;
}

#div-card-presentation-deuxieme50 {
  width: 50%;
  height: 90%;
  margin: auto;
  float: left;

}

#nom-header {


}


.lettre {
  margin-right: -10px;
}



</style>
