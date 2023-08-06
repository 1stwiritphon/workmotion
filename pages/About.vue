<template>
  <v-app>
    <Navbar/>
    <Sidebar/>
    <About/>
  </v-app>
</template>

<script>
import About from '~/components/About.vue';
import Navbar from '../components/Navbar.vue';
import Sidebar from '~/components/Sidebar.vue';
export default {
    components: { About, Navbar, Sidebar }
}
</script>

<style>

</style>