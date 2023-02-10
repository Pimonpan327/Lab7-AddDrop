<template>
    
<v-card
    theme="dark"
    flat
    rounded="0"
  >
    <v-window
      v-model="window"
      show-arrows
    >
      <v-window-item
        v-for="n in length"
        :key="n"
      >
        <v-card width="1200px" height="350px" class="d-flex justify-center align-center">
          <span class="text-h2">Drop w before 14th Febuary </span>
        </v-card>
      </v-window-item>
    </v-window>
   </v-card>
   <br>

   <v-container>
    <v-row justify="center">
        <v-col>
    <v-card
    class="mx-auto"
    max-width="400"
    elevation="11"
  >
    <v-card-text>
      <div>New of the Day</div>
      <p class="text-h4 text--primary">
        การยื่นคาดว่าจะสำเร็จการศึกษา 2/2565
      </p>
      <p>adjective</p>
      <div class="text--primary">
        สิ่งที่ต้องทำ อย่าลืม!!...
      </div>
    </v-card-text>
    <v-card-actions>
      <v-btn
        variant="text"
        color="teal-accent-4"
        @click="reveal = true"
      >
        Read More
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <v-card
        v-if="reveal"
        class="transition-fast-in-fast-out v-card--reveal"
        style="height: 100%;"
      >
        <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            การยื่นคาดว่าจะสำเร็จการศึกษา 2/2565
          </p>
          <p>
            #ยื่นคาดว่าจะสำเร็จการศึกษาออนไลน์
            #ตั้งแต่วันที่ 13 ธ.ค. 2565 - 12 มี.ค. 2566
            #ขอได้ที่ไหน เข้าได้ที่ www.education.mju.ac.th/Student/Login.aspx
            หรือสแกนคิวอาร์โค้ด
          </p>
        </v-card-text>
        <v-card-actions class="pt-0">
          <v-btn
            variant="text"
            color="teal-accent-4"
            @click="reveal = false"
          >
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-expand-transition>
  </v-card>
  </v-col>
  <br>

  <v-col>
  <v-card
    class="mx-auto"
    max-width="400"
    elevation="11"
  >
    <v-card-text>
      <div>New of the Day</div>
      <p class="text-h4 text--primary">
        ค่ายคอมแคมป์ ครั้งที่ 21
      </p>
      <p>adjective</p>
      <div class="text--primary">
         Comcamp 21...
      </div>
    </v-card-text>
    <v-card-actions>
      <v-btn
        variant="text"
        color="teal-accent-4"
        @click="reveal2 = true"
      >
        Read More
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <v-card
        v-if="reveal2"
        class="transition-fast-in-fast-out v-card--reveal"
        style="height: 100%;"
      >
        <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            Comcamp
          </p>
          <p>
            ค่ายยุวชนคอมพิวเตอร์ ครั้งที่21 Comcamp21st
            ในปีนี้จะได้เรียนรู้ปฏิบัติจริงเกี่ยวกับ IOT , Google Spreadsheet , Google Data Studio และกิจกรรมสนุกๆ
          </p>
        </v-card-text>
        <v-card-actions class="pt-0">
          <v-btn
            variant="text"
            color="teal-accent-4"
            @click="reveal2 = false"
          >
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-expand-transition>
  </v-card>
  </v-col>
  <br>

  <v-col>
  <v-card
    class="mx-auto"
    max-width="400"
    elevation="11"
  >
    <v-card-text>
      <div>New of the Day</div>
      <p class="text-h4 text--primary">
        Drop W
      </p>
      <p>adjective</p>
      <div class="text--primary">
        ช่วงวันทำการถอนรายวิชา อย่าลืม!!...
      </div>
    </v-card-text>
    <v-card-actions>
      <v-btn
        variant="text"
        color="teal-accent-4"
        @click="reveal3 = true"
      >
        Read More
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <v-card
        v-if="reveal3"
        class="transition-fast-in-fast-out v-card--reveal"
        style="height: 100%;"
      >
        <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            Drop W
          </p>
          <p>
            บอกเลิกรายวิชา โดยได้รับอักษร W ภาคเรียนที่ 2/2565 ภายในวันที่ 14 กุมภาพันธ์ 2566
          </p>
        </v-card-text>
        <v-card-actions class="pt-0">
          <v-btn
            variant="text"
            color="teal-accent-4"
            @click="reveal3 = false"
          >
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-expand-transition>
  </v-card>
  </v-col>

  </v-row>
  </v-container>
  </template>

  <script>
  export default {
    data: () => ({
      length: 3,
      window: 0,
      reveal: false,
      reveal2: false,
      reveal3: false,
    }),
  }
</script>

<style>
.v-card--reveal {
  bottom: 0;
  opacity: 1 !important;
  position: absolute;
  width: 100%;
}
</style>