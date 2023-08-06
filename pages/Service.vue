<template>
 <v-app>
    <Navbar/>
    <Sidebar/>
    <Myservice/>
 </v-app>
</template>

<script>
import Myservice from "~/components/Myservice.vue";
import Navbar from "~/components/Navbar.vue";
import Sidebar from "~/components/Sidebar.vue";
export default {
    components: { Myservice, Navbar, Sidebar }
}
</script>

<style>

</style>