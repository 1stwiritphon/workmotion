<template>
  <v-layout id="teams">
    <v-container>
      <div class="content">
        <div class="heading">
          <h1>Meet Our Team</h1>
          <p class="head-sub">
            Lorem Ipsum is simply dummy text of the printing
          </p>
            <div class="hr"></div>
        </div>
        <div class="cards">
          <v-row>
            <v-col
              cols="6"
              sm="6"
              xl="3"
              lg="4"
              v-for="card in cards"
              :key="card.id"
            >
             <div class="images">
                 <v-img class="image white--text align-end" :src="card.image">
                  <h4>{{ card.name }}</h4>
                  <p class="card-subtitle">{{ card.job }} {{ card.status }}</p>
              </v-img>
             </div>
            </v-col>
          </v-row>
        </div>
      </div>
    </v-container>
  </v-layout>
</template>

<script>
export default {
  name: 'team',
  data() {
    return {
      cards: [
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
        {
          name: 'Calla Wang',
          job: 'chief executive officer ',
          status: '(CEO)',
          image:
            'https://s3-alpha-sig.figma.com/img/b572/2438/27d69e0740d46a92db1ff2dc75094fd4?Expires=1659312000&Signature=SHKXFg005i8ICv0P-Q8tnBHa2eZW5nOD86dlfwgRMhQbUmgbGYAx~oTxIzCIr1r1wd3hW2jRR7R3jomwtjMxb7ws8I7XDwR-Hby~ztdvr0eUmXmL2FXYYjCaD19nB~0egDQqlsyQa4ovFDQNZ011QhYDTdza4o6MlhcswPLtakYyCYN7mAdaTOrbENcApVI1Xay~N8i6ZYVIP1q-k106t0mMiqwdTC8yQfNwdVoA9u2okbV2aKyUPTpLwc35PSt1Ub7YEkB~-h37LbnEXrTvzrecjgPnFO53cO1Avwj8cQIvhKWJCmDsaR6Ppee6tuoWZk1lLYgqMtTXAGmwCUEMAg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA',
        },
      ],
    }
  },
}
</script>

<style scoped>
#teams {
  background: radial-gradient(
    81.99% 81.99% at 50% 0%,
    #262a65 0%,
    #010b24 100%
  );
}
.content {
  margin: 188px 119px;
}
.heading {
  margin-bottom: 84px;
  text-align: center;
}
h1 {
  font-family: 'SF Pro Text';
  font-style: normal;
  font-weight: 800;
  font-size: 36px;
  line-height: 43px;
  margin-bottom: 21px;
  color: #42e8e0;
}
.head-sub {
  font-family: 'SF Pro Text';
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;
  margin-bottom: 19px;

  color: #ffffff;
}
.images {
  width: 261px;
  height: 373px;
 background: linear-gradient(180deg, rgba(0, 40, 150, 0) 50.11%, #000000 100%);
}
.image {
  width: 261px;
  height: 373px;
}
.hr{
width: 59px;
height: 5px;
display: inline-block;


background: #42E8E0;
}
</style>
