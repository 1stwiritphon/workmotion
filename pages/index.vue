<template>
<v-app >
  <Home/>
   <Navbar/>
   <Sidebar/>
</v-app>
</template>

<script>
import Navbar from '~/components/Navbar.vue';
import Sidebar from '~/components/Sidebar.vue';
import Home from '../components/Home.vue';

export default {
    name: "IndexPage",
    components: { Navbar, Sidebar, Home }
}
</script>

                     