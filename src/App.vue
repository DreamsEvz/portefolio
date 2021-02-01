<template>
  <v-app>

      <nav>
        <ul>
          <li>
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


    <v-card class="mx-auto" width="80%" height="500px" style="min-height: 84%">
      <v-card-title class="justify-center" style="color: #DD9D8F; font-size: 25px; margin-top: 3px;">
        Présentation personnelle
      </v-card-title>
        <v-card-text style="font-size: 15px">
          Jeune étudiant de 19 ans
        </v-card-text>
      

      <!-- <v-divider vertical width="70%" style="margin-right: auto; margin-left: auto; margin-top: 250px; "  ></v-divider> -->
      <v-img >

      </v-img>

    </v-card>
  </v-app>
</template>

<script>


export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style>

header {
  width: 100%;
  height: 150px;
  background-color: grey;
  box-shadow: 0px 5px 10px black;
}

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


#a {
  color: black;
  text-decoration: inherit;



}

#a:hover{
  border-bottom: #DD9D8F solid 3px;
  padding-bottom: 15px;
  color: #DD9D8F;

}
nav li span {
  margin-right: 250px;
  font-size: 40px;
  color : #DD9D8F;
}



</style>
