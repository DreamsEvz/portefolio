<template>
  <v-app>

      <nav>
        <ul>
          <li id="nom">
            MARCEL Evan
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



#nom {
  margin-right: 250px;
  font-size: 50px;
  color : #DD9D8F;
}

</style>
