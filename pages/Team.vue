<template>
  <v-app>
    <Navbar/>
    <Sidebar/>
    <Myteam/>
  </v-app>
</template>

<script>
import Myteam from '~/components/Myteam.vue';
import Navbar from '~/components/Navbar.vue';
import Sidebar from '~/components/Sidebar.vue';
export default {
    components: { Myteam, Navbar, Sidebar }
}
</script>

<style>

</style>