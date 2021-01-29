<template>
  <v-app>
    <header>
      <nav>
        <ul>
          <li>
            COMPÉTENCES
          </li>
          <li>
            FORMATIONS
          </li>
          <li>
            CURRICULUM VITÆ
          </li>
          <li>
            RÉALISATIONS
          </li>
          <li>
            <a href="">
              CONTACT
            </a>
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
nav a {
  display:inline-block;
  margin: 0 30px;
}
</style>
