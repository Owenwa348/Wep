<template>
  <!-- แถบ ภาพ  -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-image-container">
        <img
          src="https://img-prod.api-onscene.com/cdn-cgi/image/format=auto,width=1600/https://sls-prod.api-onscene.com/partner_files/trueidintrend/1874/S__76718085.jpg"
          class="d-block w-100"
          alt="..."
        />
        <router-link :to="{ name: 'main' }">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="32"
            height="32"
            fill="currentColor"
            class="bi bi-house house-icon"
            viewBox="0 0 16 16"
          >
            <path
              d="M8.707 1.5a1 1 0 0 0-1.414 0L.646 8.146a.5.5 0 0 0 .708.708L2 8.207V13.5A1.5 1.5 0 0 0 3.5 15h9a1.5 1.5 0 0 0 1.5-1.5V8.207l.646.647a.5.5 0 0 0 .708-.708L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.707 1.5ZM13 7.207V13.5a.5.5 0 0 1-.5.5h-9a.5.5 0 0 1-.5-.5V7.207l5-5 5 5Z"
            />
          </svg>
        </router-link>
      </div>
      <div class="carousel-caption d-none d-md-block">
        <h5>วนอุทยานภูบ่อบิด</h5>
        <p>วนอุทยานภูบ่อบิด อ.เมือง จ.เลย</p>
      </div>
    </div>
  </div>

  <!-- แถบ menu -->
  <Header_box_north_east></Header_box_north_east>

  <!-- แถบ เนื้อหา -->

  <!-- box รูปซ้าย -->
  <div class="container">
    <div class="card mb-3" style="max-width: 1500px">
      <div class="row g-0">
        <div class="col-md-4">
          <img
            src="http://i-san.tourismthailand.org/wp-content/uploads/2018/12/9283229714e07ffa9e510de121a8e72013b91357-715x475.jpg"
            class="img-fluid rounded-start"
            alt="..."
          />
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="card-title">วนอุทยานภูบ่อบิด</h5>
            <p class="card-text">
              ภูบักบิด หรือ ภูบ่บิด เป็นภูเขาเล็กๆ อยู่ห่างจากจังหวัดเลย 1 กิโลเมตร
              ด้วยระยะทางที่ใกล้จากตัวเมือง จึงนับเป็น ‘หอชมทะเลหมอกใจกลางเมือง’
              หนึ่งเดียวในประเทศไทย แถมยังเป็นขวัญใจของนักวิ่ง
              ในการเวียนมาฝึกซ้อมยามเช้ากันอยู่บ่อยๆ
            </p>
          </div>
        </div>
      </div>
    </div>

    <!--box รูปขวา-->
    <div class="card mb-3" style="max-width: 1500px">
      <div class="row g-0">
        <div class="col-md-8">
          <div class="card-body">
            <p class="card-text">
              ด้วยระยะทางเดินสู่จุดยอดที่พอเรียกเหงื่อได้กำลังดี เมื่อแลกกับวิวสวยๆ ที่ปลายทางแล้ว
              การพิชิตยอดภูบ่อบิดเพื่ออากาศบริสุทธิ์ พร้อมชมดวงอาทิตย์ท่ามกลางทะเลหมอกยามเช้า
              จัดว่าเป็นอะไรที่คุ้มค่าแก่การเดินทางมาสัมผัสหมอกกลางเมือง ณ ที่แห่งนี้
            </p>
          </div>
        </div>
        <div class="col-md-4">
          <img
            src="https://s.isanook.com/tr/0/ud/286/1434209/t2.jpg?ip/resize/w728/q80/jpg"
            class="img-fluid rounded-start"
            alt="..."
          />
        </div>
      </div>
    </div>

    <!-- สิ่งของแนะนำขาย -->
    <h1>สิ่งที่ควรเตรียมไป</h1>
    <hr />

    <div class="row row-cols-1 row-cols-md-2 g-4">
      <div
        class="card mb-3"
        style="max-width: 800px"
        v-for="(i, index) in item_advice_north_east_02_all"
        :key="index"
      >
        <div class="row g-0">
          <div class="col-md-4">
            <div class="card">
              <img :src="i.img" class="img-fluid rounded-start" alt="..." />
            </div>
          </div>

          <div class="col-md-8">
            <div class="card-body">
              <h5 class="card-title">{{ i.name }}</h5>
              <p class="card-text">{{ i.category }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <p class="card-text">
    <small class="text-body-secondary">
      <a href="https://travel.trueid.net/detail/kW22p6w5JexW">อ้างอิงมาจาก</a></small
    >
  </p>
</template>

<script setup>
import Header_box_north_east from '../north_east/Box_menu_north_east.vue'

import { ref } from 'vue'
import { item_advice_north_east_02Store } from '../north_east/index_north_east'

const item_advice_north_east_02 = item_advice_north_east_02Store()
const item_advice_north_east_02_all = ref(item_advice_north_east_02.item_advice_north_east_list_02)
</script>
