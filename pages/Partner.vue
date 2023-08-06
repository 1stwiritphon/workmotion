<template>
  <v-app>
    <Navbar/>
    <Sidebar/>
    <Mypartner/>
  </v-app>
</template>

<script>
import Mypartner from '~/components/Mypartner.vue';
import Navbar from '~/components/Navbar.vue';
import Sidebar from '~/components/Sidebar.vue';
export default {
    components: { Mypartner,Navbar, Sidebar }
}
</script>

<style>

</style>