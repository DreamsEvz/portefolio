<template>
  <v-app>

      <nav>
        <ul>
          <li class="nom-header">
            <span>
              MARCEL EVAN
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
    <v-divider style="margin-top: 50px"></v-divider>


    <v-card class="mx-auto" width="80%" height="100%" id="card-presentation" style="animation-duration: 3s ; animation-name: tranlate-left-card-presentation">
      <div id="div-card-presentation-premier50">
        <v-card-text style="font-size: 25px; text-align: center">
          Jeune étudiant de 19 ans
        </v-card-text>
      </div>
      <div id="div-card-presentation-deuxieme50">
        <img src="src/img/logo.jpg">
      </div>
      <!-- <v-divider vertical width="70%" style="margin-right: auto; margin-left: auto; margin-top: 250px; "  ></v-divider> -->

    </v-card>
  </v-app>
</template>

<script>


export default {
  name: 'App',

  data: () => ({

  }),


};
</script>

<style>

nav {
  padding: 0;
  text-align: center;
  margin: 30px 0 0;
}
nav li {
  display: inline;
  list-style: none;
  font-size:15px;
  padding: 30px;

}

/* Les id "a" correspondent à plusieurs élément car le code css ci-dessous ne fonctionne pas en appelant l'élément ou en utilisant une class */
#a {
  color: black;
  text-decoration: inherit;
  transition-property: padding-bottom;
  transition-duration: 0.5s;
  padding-bottom: 0px;
}

#a:hover{
  border-bottom: #DD9D8F solid 3px;
  padding-bottom: 15px;
  color: #DD9D8F;


}
nav li span {
  margin-right: 200px;
  font-size: 40px;
  color : #DD9D8F;
  animation-duration: 3s;
  animation-name:translate-left-nom;
}


@keyframes tranlate-left-card-presentation {
  from {
    opacity: 0;
  }
  to {
   opacity: 1;
  }
}

@keyframes translate-left-nom {
  from {
    opacity: 0;
  }
  to {
    opacity:1;
  }
}

#div-card-presentation-premier50{
  width: 50%;
  height: 90%;
  margin: auto;
  float: left;
}
#div-card-presentation-deuxieme50{
  width: 50%;
  height: 90%;
  margin: auto;
  float: left;

}


</style>
