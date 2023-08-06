<template>
  <v-layout id="contact">
    <v-container>
      <div class="content">
        <h1>Write us</h1>
        <div class="hr"></div>

        <v-row dense>
          <v-col cols="12" xl="4" md="6">
            <form class="mt-12">
              <label for="message">message</label> <br />
              <textarea
                name="message"
                style="
                  width: 500px;
                  height: 100px;
                  border: none;
                  border-bottom: 1px solid white;
                  color: grey;
                "
              >
Write text here</textarea
              >
              <br />
              <label for="name">Name</label><br />
              <input
                type="text"
                id="name"
                name="name"
                style="
                  width: 500px;
                  height: 50px;
                  border-bottom: 1px solid white;
                  color: #ffffff;
                "
              /><br />

              <label for="email">Email</label><br />
              <input
                type="email"
                id="email"
                name="email"
                style="
                  width: 500px;
                  height: 50px;
                  border-bottom: 1px solid white;
                  color: #ffffff;
                "
              />
              <br />

              <input type="checkbox" id="check" name="check" class="mt-7" />
              <label for="check">I am not a robot</label>
            </form>
            <v-btn block width="500px" height="50px" style="background: rgba(245, 53, 83, 0.5);" class="mt-7 "> submit </v-btn>
          </v-col>

          <v-col cols="">
            <div class="maps">
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3874.4598500137463!2d100.56242531474973!3d13.811403390308913!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x30e29d4c0c3eef37%3A0x77dc9975aa56a5a1!2sWorkmotion%20Corp%20Office!5e0!3m2!1sth!2sth!4v1656928817840!5m2!1sth!2sth"
                width="600px"
                height="330px"
                style="border: 0"
                loading="lazy"
                allowfullscreen
              ></iframe>
              <br />
             <div class="block" style='width: 400px;'>
               <div class="location d-flex">
                <div><v-icon>mdi-map-marker-outline</v-icon></div>
                <div>
                  <p>
                    บริษัท เวิร์คโมชั่น ครีเอทีฟ จำกัด (Workmotion Corp)
                    ตึกพร้อมพันธุ์ 1 ชั้น 4 ซอย ลาดพร้าว 15 เขตจตุจักร
                    กรุงเทพมหานคร 10900
                  </p>
                </div>
              </div>
              <div class="email d-flex">
                <div><v-icon>mdi-email</v-icon></div>
                <div>
                  <p>
                    workmotion@crop.co.th
                  </p>
                </div>
              </div>
              <div class="number d-flex">
                <div><v-icon>mdi-phone</v-icon></div>
                <div>
                  <p>
                    02-147-0983
                  </p>
                </div>
              </div>
             </div>
            </div>
          </v-col>
        </v-row>
      </div>
    </v-container>
  </v-layout>
</template>

<script>
export default {
  name: 'contact',
}
</script>

<style scoped>
#contact {
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
  font-family: 'Open Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 64px;
  line-height: 87px;

  color: #ffffff;
}
.hr {
  width: 150px;
  height: 5px;

  background: #f53553;
}

.maps {
  width: 700px;
  height: 390px;
  border-left: 2px solid #fff;
  padding: 0 20px;
  margin-left: 100px;
}
</style>