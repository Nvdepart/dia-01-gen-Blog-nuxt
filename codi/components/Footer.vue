<template>
    <v-card 
        tile flat 
        class="pa-md-10 pa-5 text-center" 
        color="surface">
    <h2 class="text-md-h5 font-weight-bold">Atlas-Expo</h2>
    <br>
    <v-btn v-for="s in sm" 
        :key="s.icon" 
        icon 
        :to="s.link" 
        fab 
        color="surface" 
        class="mr-2"
        depressed>
        <v-icon >{{s.icon}}</v-icon>
    </v-btn>
    </v-card>
</template>

<script>
    export default {
        data(){
            return {
                sm:[
                {
                    icon:"mdi-facebook", link:"http://www.facebook.com",
                },
                {
                    icon:"mdi-instagram", link:"http://www.instagram.com",
                },
                {
                    icon:"mdi-twitter", link:"http://www.twitter.com",
                },
                {
                    icon:'mdi-youtube', link:'http://www.youtube.com',
                }
                ]
            }
        }
    }
   
</script>

<style scoped>

</style>