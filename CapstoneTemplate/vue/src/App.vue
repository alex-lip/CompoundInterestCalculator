<!-- Main Application Template. 
     Note that you have classes from bootstrap available to you.
     See https://getbootstrap.com/docs/4.5/getting-started/introduction/ for reference on bootstrap -->
<template>
  <div id="app" class="container-fluid">
    
    <nav class="navbar navbar-light bg-light justify-content-between">
      <a class="navbar-brand">
        🧮 Margin and Markup Calculator
      </a>
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
  //background-color: rgb(255, 255, 255);
  padding-bottom: 50px;
}

#nav {
  background-color: white;
}

.navbar-brand {
  color: black;
}

</style>