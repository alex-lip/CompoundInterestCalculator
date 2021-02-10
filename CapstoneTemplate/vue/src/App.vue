<!-- Main Application Template. 
     Note that you have classes from bootstrap available to you.
     See https://getbootstrap.com/docs/4.5/getting-started/introduction/ for reference on bootstrap -->
<template>
  <div id="app" class="container-fluid"> <!-- If you start to get random styling you don't like, remove container from this div -->
    <nav class="navbar navbar-light bg-light justify-content-between">
      <router-link class="navbar-brand" v-bind:to="{ name: 'home' }">
        Margin Calculator
      </router-link>
      </nav>
      <router-view />
    
    
  </div>
</template>

<script>
export default {
  
}
</script>

<!-- Application-Wide Styles go here. 
     Any valid CSS or SCSS is allowable here. See https://sass-lang.com/documentation/style-rules for info on SCSS -->
<style lang="scss">

#app {
  font-family: Arial, Helvetica, sans-serif;
}

.container-fluid {
  background-color: rgb(240, 240, 240);
  padding-bottom: 50px;
}

#nav {
  background-color: white;
}

.navbar-brand {
  color: black;
}

</style>