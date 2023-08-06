<template>
  <v-layout id="articles">
    <v-container>
      <div class="content">
      <h1>Articles Us</h1>
      <v-row>
        <v-col
          cols="12"
          sm="6"
          xl="3"
          lg="4"
          v-for="card in cards"
          :key="card.id"
        >
          <div class="card">
            <div class="card-header">
              <img class="image" @click="dialog = true" :src="card.image" />
            </div>
            <div class="card-body">
              <h4>{{ card.title }}</h4>
              <p class="card-subtitle">{{ card.sub }}</p>
              <p class="card-date">{{ Time() }}</p>
            </div>
          </div>

          <v-dialog v-model="dialog">
            <div class="dialog">
              <img
                class="dialog-image"
                @click="dialog = true"
                :src="card.image"
              />
              <div class="dialog-content">
                <h4 class="dialog-title">{{ card.title }}</h4>
                <p class="dialog-p">{{ card.dialog }}</p>
              </div>
            </div>
          </v-dialog>
        </v-col>
      </v-row>
      </div>
    </v-container>
  </v-layout>
</template>

<script>
export default {
  name: "articles",
  data() {
    return {
      dialog: false,
      cards: [
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        {
          title: "Digital Maketing",
          sub: "Lorem Ipsum is simply dummy text of the printing and typesetti copyLorem Ipsum is simply dummy text of the printing and typesetti copy",
          image:
            "https://s3-alpha-sig.figma.com/img/acfb/9a09/0f34a0c9385594bfca15776830ea07b7?Expires=1659312000&Signature=HGNFJAeBTRt18uiK2fAi~sDv7T-xYQfHSmge40WMNIzXP-TuXBtKHUi09gxxAiAY-3DnWL2vun2pSKsVRjcAFB9OI0iefhHKqlmVGFIyGmi7gQ7CQI8EF5~1tDjSS~lFr-U9xmsmHm8hC1JLygDWedp6OZwto8muOOXbh6sTOn8r9Vcx-eJhKp0gYyX8tdOH0~Flzi032BrcstCN6geVNPjOTqqoFs7gNfpqC1vmpj8yKsnxLrgGkz4NKC5i~3kan32HFbWlV6sNcrc~w-DrWlHDFdJWG2QYyrUJ3DAMKKXS-ryWD9l6T1AkHMfaL6UgsQ7qTavgqqaOddFh5U62Qg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          dialog:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industrys standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
        },
        
      ],
    };
  },
  methods: {
    Time() {
      const current = new Date();
      const date =
        current.getDate() +
        "-" +
        (current.getMonth() + 1) +
        "-" +
        current.getFullYear();
      const time = current.getHours() + ":" + current.getMinutes();
      const dateTime = date + " " + time;

      return dateTime;
    },
  },
};
</script>

<style scoped>
#articles {
   background: radial-gradient(
    81.99% 81.99% at 50% 0%,
    #262a65 0%,
    #010b24 100%
  );
}
.content{
  margin: 188px 41px;
}
h1 {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 600;
  font-size: 96px;
  line-height: 115px;
  margin-bottom: 30px;
  margin-left: 15px;

  color: #ffffff;
}
.text-head h1 {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 600;
  font-size: 96px;
  line-height: 115px;
  color: #ffffff;
}
.card {
  width: 305px;
  background: #ffffff;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  overflow: hidden;
}
.card-header .image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
.card-body {
  display: flex;
  flex-direction: column;
  padding: 15px;
}
.card-body h4 {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 800;
  font-size: 14px;
  line-height: 17px;

  color: #262a65;
}
.card-subtitle {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 400;
  font-size: 11px;
  line-height: 13px;
  margin-top: 5px;
  color: #000000;
}
.card-date {
  font-family: "Open Sans";
  font-style: normal;
  font-weight: 400;
  font-size: 8px;
  line-height: 11px;
  color: #999999;
  margin-top: 7px;
}

.dialog {
  position: absolute;
width: 1256px;
height: 747px;
left: 20%;
top: 10%;

  background: #ffffff;
  border-radius: 20px;
}
.dialog-image {
  width: 1256px;
  height: 414px;

  border-radius: 20px 20px 0px 0px;
}
.dialog-content{
  margin-left: 40px;
}
.dialog-title {
  width: 297px;
  height: 49px;

  font-family: "Open Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 36px;
  line-height: 49px;
  color: #262a65;
}
.dialog-p {
  width: 1171px;
  height: 125px;

  font-family: "Open Sans";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 25px;

  color: #000000;
}
</style>