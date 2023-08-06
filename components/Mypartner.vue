<template>
  <v-layout id="partners">
    <v-container >
        <div class="content">
      <h1>Our Partners</h1>
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
            <div class="card-image">
              <img
                :src="card.image"
                :width="card.width"
                :height="card.height"
              />
            </div>

            <div class="card-content">
              <h4>{{ card.title }}</h4>
              <p class="card-subtitle">{{ card.sub }}</p>
            </div>
            <p class="card-foolter">ประเภท : {{ card.type }}</p>
          </div>
        </v-col>
      </v-row>
      <img
        src="https://s3-alpha-sig.figma.com/img/db3f/93a3/d581cbec27a49567ea47eb7265089087?Expires=1659312000&Signature=PWOfJNlcjs2zbIHlmLw7Ve2TPJI~52B57CmyHwZ5sTDLjjsE-ZaBJm6nYYtikSdPjy2WfHqCyfuh4pt~ZzA3VbGl91zZwEk3a-y~4XA8o2T7eGq8d7zzwxaKk25vSMzKTGzI7jMUWbqrNbdvePRMzoD-93D9EpsfgOgtWyKD9L33zC7lHe12HhnsFdcKjAw8EEDTD1cPOvGMMbSqaStMVSHESB6hcHrL7~zWv4esURBgpzbPanjh8NKVh0oDWFCbjllnH5d8bo-kE3UvetmOr7uUOan5-tJEuholZ9ogfxHV4u7pcI~sOiwulOINnFuVf7u7j7ebheK9SIYKitf0Gg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA"
        alt=""
        width="841px"
        height="194px"
      />
        </div>
    </v-container>
  </v-layout>
</template>

<script>
export default {
  name: "partner",
  data() {
    return {
      cards: [
        {
          title: "MuayThai lyarin ",
          sub: "Application สำหรับผู้ที่หลงไหลศาสตร์ มวยไทย และมีข่าวสารการมวย ส่งตรงจากเซียนมวย",
          image:
            "https://s3-alpha-sig.figma.com/img/e6e2/dc35/36420b10499ebfd69cde77c0224d56d0?Expires=1659312000&Signature=gnucUxg4Kcb7~ATg0VIejiZ6J3rUu6NOBq-iKlXSiU3GNz3aZeWAUqgMUw4X8TJVQ-MplDYK1E4d4yI30hRM4a0CsMRr42Dy-ifBXtMMKKZc1XRvdpWiozuwKeZRUCQ~ki78~mSWFVIQloFdjpP8VilAczr4UwsNX1mNch8Zt4XAJyEAN1PWvQhy9jhSABybECzYcbGg1iWW~IiyLCSLRjLI~e1EIwC7x6j0v8sVdx~HdRdabwpGPUyFBt0xqj0q9grBIp8dS4VFsfUZ5C5AbZivdZjQx-nbmAVOZpVz3KWYAYXgYV102CqX7XrdAjMY~7ChCJ7GiQP8tZb532RBzg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          width: "208px",
          height: "109px",
          type: "Android and iOS",
        },
        {
          title: "wExib",
          sub: "platform ที่ให้บริการ Live streaming event สำหรับผู้ที่ต้องการชม Exibition ผ่าน online",
          image:
            "https://s3-alpha-sig.figma.com/img/a745/3a2c/10a5e5af8aa9cc5573dc4b8a9e4935e8?Expires=1659312000&Signature=bwxUGPzPQfCdna6KrUA-e4wCxbtFFVuejhNBeJYeVnNy~0HEMEXxF7r4bXkzGpTJLYO6muKPNsjSyy7JV-eKDAutvCt3f-EjfZkEbxRdy0qwDijAPQcwBwnUG8xZKNoZOH1qIJxf~B9HetAzNEcYNE7LZQKmkM3xzb5ZgytCY-vAemuI13OhDoV99FKTev0evKcBSBEZmuxJyRhyARxrTVPhXNUj~gaq8OStqjKeaDBrB8wr7FKjpn6~aUqfkFhT2XakSe5WPy64f2BFGCIuagwiW8bSWQVXeTPQmrB3tNnG3r0AphA7-Vzv27w5Ut8gxaLhrVJq1Dd7~dTgOshEYg__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          width: "208px",
          height: "67px",
          type: "Platform Website",
        },
        {
          title: "Naina:dee",
          sub: "Platform ที่รวบรวมและให้บริการของนายหน้า และทรัพย์ของนายหน้า",
          image:
            "https://s3-alpha-sig.figma.com/img/e0c7/783b/e1def41adc92bbb8301ed69dc242d642?Expires=1659312000&Signature=Hu~wX7nEo-ogdxz4TnaiHj4eOX47zJbltT4Jt2PllW62aoS8C4J1LO14~Us5txAZhBYfILIdxwJvJ2pmLGINkt-jXQmFr89m8Dyq6WCquM995w~0Y-xGDHdD4sivKaLxeDVP8qbLDDPsSx5KgHhuyjtoudKYxHmSSMcugm9h2h3PSeI27V59076tEtoKIdMNFSQDpyh9XVmcLr4B27-3wJR7Ewqv1A7p7l83x~OdkWroxkXhTJvdWx5i~xgJ5O94OH6Er7eKRZnoPqUQE5O2Mr~QAmKRXL4sHKRgoH60JYeQ8G12GWAB6GcXKrNdobfIMIZB74vl2XWq2rqcoScDSA__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          width: "208px",
          height: "33px",
          type: "Android and iOS",
        },
        {
          title: "Boonumpar ERP ",
          sub: "ระบบบริหารจัดการ ERP แบบonline และ เครื่องมือ ในการวิเคราห์ข้อมูลจากระบบ",
          image:
            "https://s3-alpha-sig.figma.com/img/bec3/506e/acb18378cb8e86af7b10c53e337af706?Expires=1659312000&Signature=RJF498cCsOfhUeUYkAtVGwADdaxNjtkHB9pXQaX1BtsuwLCpue5IXU50vXr4ZmFlasfamBoaEPp-EuVWIrPRc9gyil9M1fnEdrmKRaDqSCWBdVJ3V~7Va5CMXES1Tx-OmBltQ3xH69~m6Ff0PPhWotBwQxQiFGcCPFY2~sv7Z-YJYOHsr9bPAtIviJvrt-hcywYQgr-9FzDiUg7zVv0A2K3uz1S5keG1FvDlB0WGkjwCTBNE~Dp25uSocMRid3pKza-Ahd0KaXrww099Y1eCcFkV~5Hed6cQNuJtQ8aDvTyXaAB1Ginc-caYKuhnVKqRxrgluZBEkmSfxTmaJ6aJcQ__&Key-Pair-Id=APKAINTVSUGEWH5XD5UA",
          width: "100px",
          height: "148.65px",
          type: "Online Platform",
        },
      ],
    };
  },
};
</script>

<style scoped>
#partners{
  height: auto;
   background: radial-gradient(
    81.99% 81.99% at 50% 0%,
    #262a65 0%,
    #010b24 100%
  );
}
.content {
  margin: 188px 60px;
}
h1 {
  width: 644px;
  height: 115px;

  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 600;
  font-size: 96px;
  line-height: 115px;
  
  margin-bottom: 30px;

  color: #ffffff;
}
.card {
  width: 300px;
  height: 437px;
  background: #262a65;
  box-shadow: 0px 0px 50px rgba(0, 0, 0, 0.3);
  border-radius: 10px;
}
img {
  margin-top: 60px;
}
h4 {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 800;
  font-size: 24px;
  line-height: 29px;
  margin-bottom: 20px;
  color: #ffffff;
}
p {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;
  margin-bottom: 30px;
  color: #ffffff;
}
.card-image {
  text-align: center;
  width: 100%;
  height: 220px;
}
.card-content {
  margin: 20px 30px 30px 30px;
  width: 246px;
  height: 70px;
}
.card-foolter {
  margin: 50px 0 0 30px;
  width: 246px;
}
</style>