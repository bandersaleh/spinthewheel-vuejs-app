<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/student">Audience Window</router-link> |
    <router-link to="/controls">Controls Window</router-link>
  </nav>
  <router-view/>
  <footer>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    <br>
    <br>
    <p>© 2023 Bander Saleh. All rights reserved.</p>
  </footer>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: grid; 
  grid-template-columns: 1fr; 
  grid-template-rows: 1fr 6fr 1fr; 
  gap: 0px 0px; 
  grid-template-areas: 
    "nav"
    "router-view"
    "footer"; 
  grid-area: Index\.html; 
}

nav {
  grid-area: nav;
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.router-view { grid-area: router-view; }

footer {
  grid-area: footer;
  /* padding: 30px 0px 90% 0px; */
}

footer a {
  font-weight: bold;
  color: #2c3e50;
}

footer a.router-link-exact-active {
  color: #000000;
}

</style>