<template>
  <div class="service">
    <v-row >
      <v-col
        cols="6" sm="6" xl="4" lg="6"
        class="card-service"
        v-bind:class="card1 ? 'color-on' : 'color-off'"
      >
        
          <div class="card"  >
            <div class="animation">
              <img v-show="card1" src="@/assets/image/service-1.png" alt="" />
            </div>
            <div class="num">01</div>
            

            <div v-bind:class="card1 ? 'hr-on' : 'hr-off'"></div>

            <div class="profile" color="red"></div>

           
            <v-template >
               <div class="detail"  >
              <h2>Digital Transformation Consultant and Execution Expert</h2>
              <v-expand-transition>
                <div v-show="card1">
                  <v-card-text>
                    <li>
                      ให้คำปรึกษา Digital Transformation ทีมงานที่มีความเข้าใจ
                      และช่วยพัฒนาอย่างใกล้ชิด
                    </li>
                    <div class="heading">Data Diven and Applicable</div>
                    <li>
                      วิเคราะห์ข้อมูลผู้ใช้ Data
                      เป็นข้อมูลขับเคลื่อนและปรับใช้อย่างเหมาะสม
                    </li>
                  </v-card-text>
                </div>
              </v-expand-transition>
            </div>
            </v-template>
           
          </div>
        <div class="foolter">
          <v-btn text color="#42E8E0" width="100" @click="card1 = !card1">
            {{ card1 ? "CLOSE" : "READ MORE" }}
          </v-btn>

          <v-icon icon color="#42E8E0" outlined @click="card1 = !card1">{{
            card1 ? "mdi-arrow-left-drop-circle" : "mdi-arrow-right-drop-circle"
          }}</v-icon>
        </div>
      </v-col>


      <v-col
         cols="6" sm="6" xl="4" lg="6"
        class="card-service"
        v-bind:class="card2 ? 'color-on' : 'color-off'"
      >
        <div class="content">
          <div class="card"  >
            <div class="num">02</div>

            <div v-bind:class="card2 ? 'hr-on' : 'hr-off'"></div>

            <div class="profile" color="red"></div>

            <div class="animation">
              <img v-show="card2" src="@/assets/image/service-2.png" alt="" />
            </div>
            <v-template >
               <div class="detail"  >
              <h2>Platform Application Development</h2>
              <v-expand-transition>
                <div v-show="card2">
                  <v-card-text>
                    <li>
                      พัฒนาระบบซอฟแวร์และออกแบบเว็ปไซร์
                    </li>
                    <li>
                      ออกแบบดยคำนึง UX/UI ในการใช้งาน
                    </li>
                    <li>
                      พัฒนาแอพลิเคชั่น iOS, Android
                    </li>
                    <li>
                    พัฒนา​ ERP พื้นฐาน Odoo
                    </li>
                    <div class="heading">Smart Device supply and Helpdesk support</div>
                    <li>
                     จัดหาอุปกรณ์ Smart Device และทีม support
                    </li>
                  </v-card-text>
                </div>
              </v-expand-transition>
            </div>
            </v-template>
           
          </div>
        </div>

        <div class="foolter">
          <v-btn text color="#42E8E0" width="100" @click="card2 = !card2">
            {{ card2 ? "CLOSE" : "READ MORE" }}
          </v-btn>

          <v-icon icon color="#42E8E0" outlined @click="card2 = !card2">{{
            card2 ? "mdi-arrow-left-drop-circle" : "mdi-arrow-right-drop-circle"
          }}</v-icon>
        </div>
      </v-col>


      <v-col
         cols="6" sm="6" xl="4" lg="6"
        class="card-service"
        v-bind:class="card3 ? 'color-on' : 'color-off'"
      >
        <div class="content">
          <div class="card"  >
            <div class="num">03</div>

            <div v-bind:class="card3 ? 'hr-on' : 'hr-off'"></div>

            <div class="profile" color="red"></div>

            <div class="animation">
              <img v-show="card3" src="@/assets/image/service-3.png" alt="" />
            </div>
            <v-template >
               <div class="detail"  >
              <h2>Digital Sales and Marketing Strategy </h2>
              <v-expand-transition>
                <div v-show="card3">
                  <v-card-text>
                    <li>
                      ให้บริการวิเคราะห์และวางกลยุทธ์ธุรกิจ
                    </li>
                    <li>
                      ให้บริการทำ Communication content
                    </li>
                    <li>
                      ให้บริการทำ Graphic Design
                    </li>
                    <li>
                     ให้บริการยิง Ads และวิเคระห์ผลลัพธ์
                    </li>
                    <li>
                      วิเคราะห์การใช้ช่องทาง Online ให้เหมาะกับธุรกิจ
                    </li>
                  </v-card-text>
                </div>
              </v-expand-transition>
            </div>
            </v-template>
           
          </div>
        </div>

        <div class="foolter">
          <v-btn text color="#42E8E0" width="100" @click="card3 = !card3">
            {{ card3 ? "CLOSE" : "READ MORE" }}
          </v-btn>

          <v-icon icon color="#42E8E0" outlined @click="card3 = !card3">{{
            card3 ? "mdi-arrow-left-drop-circle" : "mdi-arrow-right-drop-circle"
          }}</v-icon>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>

export default {
  name: "service",
  data: () => ({
    card1: false,
    card2: false,
    card3: false,
  }),
};
</script>

<style scoped>
.card-service {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.card {
    margin-top: 191px;
  margin-left: 30px;
  position: relative;
  overflow: hidden;
  width: 96%;
  height: 1080px;
}
.num {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 21px;
  margin-bottom: 40px;

  color: #ffffff;
}
.hr-off {
  width: 22px;
  height: 3px;
  background: #fff;
}
.hr-on {
  width: 90px;
  height: 3px;
  background: #f53553;
}
.color-on {
  background: #08195a;
  box-shadow: 15px 0px 100px rgba(0, 0, 0, 0.3);
}
.color-off {
  background: radial-gradient(
    81.99% 81.99% at 50% 0%,
    #262a65 0%,
    #010b24 100%
  );
}
.animation img {
  position: absolute;
width: 218px;
height: 330px;
left: 290px;
top: 0px;
}
.profile {
  width: 188px;
  height: 188px;
  left: 420px;
  top: 315px;
  margin-top: 60px;
  margin-bottom: 60px;
  border: 2px solid rgba(196, 196, 196, 0.6);
  border-radius: 50%;
}
.detail{
  width: 430px;
}
h2 {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 800;
  font-size: 36px;
  line-height: 43px;

  /* #FFFFFF */

  color: #ffffff;
}
li {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 17px;
  margin-top: 30px;
  color: #ffffff;
}
.heading {
  font-family: "SF Pro Text";
  font-style: normal;
  font-weight: 800;
  font-size: 18px;
  line-height: 21px;
  margin-top: 20px;
  margin-bottom: 15px;
  /* #FFFFFF */

  color: #ffffff;
}
.foolter {
  margin-bottom: 110px;
  margin-left: 30px;
}
</style>