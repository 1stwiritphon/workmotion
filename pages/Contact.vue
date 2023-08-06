<template>
  <v-app>
    <Mycontact/>
    <Navbar/>
    <Sidebar/>
  </v-app>
</template>

<script>
import Mycontact from '~/components/Mycontact.vue';
import Navbar from '~/components/Navbar.vue';
import Sidebar from '~/components/Sidebar.vue';
export default {
    components: { Mycontact, Navbar, Sidebar }
}
</script>

<style>

</style>