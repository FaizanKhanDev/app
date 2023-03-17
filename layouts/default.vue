<template>
  <v-app>
    <Navbar />
    <Appbar />
    <v-main>
        <v-container fluid>
            <Nuxt/>
        </v-container>  
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar';
import Appbar from '@/components/Appbar';
import Footer  from '@/components/Footer';
export default {
  comments:{
    name:'Navbar',
    name:'Appbar',
    name:'Footer',
  }
}
</script>
