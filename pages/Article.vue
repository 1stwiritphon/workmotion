<template>
  <v-app>
    <Navbar/>
    <Sidebar/>
    <Myarticle/>
  </v-app>
</template>

<script>
import Myarticle from "~/components/Myarticle.vue";
import Navbar from "~/components/Navbar.vue";
import Sidebar from "~/components/Sidebar.vue";
export default {
    components: { Navbar, Myarticle, Sidebar }
}
</script>

<style>

</style>