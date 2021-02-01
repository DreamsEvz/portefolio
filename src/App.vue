<template>
  <v-app>
    <header>
      <nav>
        <ul>
          <li>
            <v-btn href="" style="font-size: 20px; background-color: green">
              COMPETENCES
            </v-btn>
          </li>
          <li>
            <v-btn  href="" style="font-size: 20px; background-color: green">
              FORMATIONS
            </v-btn>
          </li>
          <li>
            <v-btn  href="" style="font-size: 20px; background-color: green">
              CURRICULUM VITÆ
            </v-btn>
          </li>
          <li>
            <v-btn  href="" style="font-size: 20px; background-color: green">
              RÉALISATIONS
            </v-btn>
          </li>
          <li>
            <v-btn href="" style="font-size: 20px; background-color: green">
              CONTACT
            </v-btn>
          </li>
        </ul>
      </nav>


    </header>
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
  margin: 50px 0 0;
}
nav li {
  display: inline;
  list-style: none;
  font-size:25px;
  padding: 30px;

}

nav v-btn:hover {
  background-color: grey;
}



</style>
