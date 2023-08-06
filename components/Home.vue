<template>
  <v-layout class="home">
    <div class="content">
      <h3>We provide services and consulting.</h3>
      <h1>
        Digital <br />
        Transformation Expert
      </h1>
      <div class="group-1">
        <p>Develop software</p>
        <p>Website</p>
        <p>Application IOS, Android</p>
        <p>ERP Odoo</p>
        <p>Marketing Online</p>
        <p>Marketing Online</p>
        <p>Plane Marketing</p>
        <p>Analyzing Ads Advertising</p>
      </div>
      <v-group class="d-flex mt-12">
        <v-btn tile outlined color="#F53553" white--text width="200px" height="80px" to="/service">read more </v-btn>
        <v-btn tile width="100px" height="80px" color="#F53553" to="/service"><v-icon >mdi-play</v-icon></v-btn>
      </v-group>  
    </div>
  </v-layout>
</template>

<script>
export default {
  name: 'home',
}
</script>

<style scoped>
.home {
  background: radial-gradient(
    81.99% 81.99% at 50% 0%,
    #262a65 0%,
    #010b24 100%
  );
}
.content {
  margin-top: 188px;
}
h3 {
  font-family: 'SF Pro Text';
  font-style: normal;
  font-weight: 300;
  font-size: 40px;
  line-height: 48px;
  /* identical to box height */

  color: #ffffff;
}
h1 {
  font-family: 'SF Pro Text';
  font-style: normal;
  font-weight: 600;
  font-size: 96px;
  line-height: 115px;
  margin-top: 17px;

  color: #ffffff;
}
.group-1 {
  display: flex;
  flex-wrap: wrap;
  width: 780px;
  margin-top: 32px;
}
p {
  margin-right: 30px;

  font-family: 'SF Pro Text';
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 24px;
  color: #ffffff;
}
</style>
                     