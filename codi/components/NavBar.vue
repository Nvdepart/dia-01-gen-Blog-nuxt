<template>
      <div>
        <v-app-bar  color="surface" height="80" class="el" app 
        :style="{padding: $vuetify.breakpoint.mdAndUp ? '0px 100px' :''}">
          <v-toolbar-title 
            @click="$router.push('/')" 
            class="text-md-h5 font-weight-bold pointer">
            Atlas-Expo
          </v-toolbar-title>
          <v-spacer></v-spacer>
          <v-btn icon>
            <v-icon size="20" fab>mdi-store-outline</v-icon>
          </v-btn>
          <v-btn icon>
            <v-icon size="20" fab>mdi-cart-outline</v-icon>
          </v-btn>
          <v-divider vertical class="mx-md-5 mx-2"></v-divider>
          
          <v-btn icon>
            <v-icon size="20" fab>mdi-brightness-6</v-icon>
          </v-btn>
        </v-app-bar>
      </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 70px;
    font-weight: lighter;
    letter-spacing: 0.5px;
  }
  .nav .logo {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .nav .logo .subheader {
    opacity: 0.70;
    font-size: 0.9rem;
    color: white;
  }
  .nav .nav-content {
    font-size: 1rem;
  }
  .nav-content ul {
    display: flex;
    list-style: none;
  }
  .nav-content ul li {
    padding: 2px 10px;
  }
  .nav-content ul li:not(:first-of-type) {
    border-left: 1px solid rgb(255, 255, 255, 0.2);
  }
</style>