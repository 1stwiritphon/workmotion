<template>
  <div id="navbar">
    <v-navigation-drawer app floating width="370px">
      <div class="side-l">
        <div class="image">
          <img src="@/assets/image/logo.png" alt="" width="120px" />
        </div>

        <div>
          <v-btn class="btn1" icon outlined>
            <v-icon color="white">mdi-play mdi-rotate-180</v-icon>
          </v-btn>
          <v-btn class="btn2" icon outlined to="/service">
            <v-icon color="white">mdi-play</v-icon>
          </v-btn>
        </div>
      </div>
    </v-navigation-drawer>

    <v-navigation-drawer
      app
      mini-variant
      right
      mini-variant-width="100"
      floating
    >
    <div class="side-r">
        <div>
            <v-icon color="white" class="ml-7 mt-10">mdi-menu</v-icon>
          </div>

          <div>
              <a href="" class="display-1 white--text ml-7">03</a>
          </div>

          <div class="icons ml-7">
            <v-col cols="12" v-for="icon in icons" :key="icon.id">
              <v-btn icon dark x-small>
                <v-icon small>{{ icon.i }}</v-icon>
              </v-btn>
            </v-col>
          </div>
    </div>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: "sidebar",
  data() {
    return {
      icons: [
        { i: "mdi-twitter" },
        { i: "mdi-facebook" },
        { i: "mdi-youtube" },
        { i: "mdi-instagram" },
      ],
    };
  },
};
</script>

<style scoped>
.side-l {
  background: radial-gradient(
    81.99% 81.99% at 50% 0%,
    #262a65 0%,
    #010b24 100%
  );
  width: 370px;
  height: 100vh;
}
.side-r{
     background: radial-gradient(
    81.99% 81.99% at 50% 0%,
    #262a65 0%,
    #010b24 100%
  );
  width: 100px;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.icons a {
  text-decoration: none;
}
.image {
  position: absolute;
  max-width: 120px;
  width: 100%;
  height: 41px;
  left: 80px;
  top: 40px;
}
.btn1 {
  position: absolute;
  width: 80px;
  height: 80px;
  left: 80px;
  top: 500px;

  border: 3px solid rgba(255, 255, 255, 0.5);
}
.btn2 {
  position: absolute;
  width: 80px;
  height: 80px;
  left: 170px;
  top: 500px;

  border: 3px solid red;
}
</style>