<script setup>
import Header_box_south from '../south/Box_menu_south.vue'
import { ref } from 'vue'
import { Otop_southStore } from '../../stores/All_product'

const otop_southStore = Otop_southStore()
const otop_south_all = ref(otop_southStore.Otop_south_list)
</script>

<template>
  <!-- แถบ ภาพ  -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-image-container">
        <img
          src="https://www.suratthanitourism.com/wp-content/uploads/2019/08/%E0%B8%AD%E0%B8%B8%E0%B8%97%E0%B8%A2%E0%B8%B2%E0%B8%99%E0%B8%98%E0%B8%A3%E0%B8%A3%E0%B8%A1%E0%B9%80%E0%B8%82%E0%B8%B2%E0%B8%99%E0%B8%B2%E0%B9%83%E0%B8%99%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87_06.jpg"
          class="d-block w-100"
          alt="..."
          height="550"
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
        <h5 class="display-3">อุทยานธรรมเขานาในหลวง อ.พนม จ.สุราษฎร์ธานี</h5>
        <p class="h4">อุทยานธรรมชาติที่สวยและงดงามเหมาะแก่การมาเยี่ยมชม ซักครั้ง</p>
      </div>
    </div>
  </div>

  <!-- แถบ menu -->
  <Header_box_south></Header_box_south>

  <div class="container">
    <!-- สิ่งของแนะนำขาย -->
    <h1 class="textcenter"><strong>แนะนำสินค้า</strong></h1>
    <hr />


  
      <div class="row row-cols-1 row-cols-md-2 g-4">
        <div class="col" v-for="(i, index) in otop_south_all" :key="index">
          <div class="card">
            <img :src="i.img" class="card-img-top" alt="..." />
            <div class="card-body">
              <h5 class="card-title">
                <strong>{{ i.name }}</strong>
              </h5>
              <p class="card-text">
                <strong>ประเภท: {{ i.category }}</strong>
              </p>
              <p class="card-text">
                <strong>ราคา:{{ i.price }} บาท</strong>
              </p>
              <p class="card-text">{{ i.text }}</p>
              <button type="button" class="btn btn-primary">ลงตะกร้า</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    
  <p class="card-text">
    <small class="text-body-secondary">
      <a href="https://www.thairath.co.th/lifestyle/travel/thaitravel/2708365">
        ขอบคุณข้อมูลอ้างอิงจาก
      </a></small
    >
  </p>
  <p class="card-text">
    <small class="text-body-secondary">
      <a href="https://palanla.com/th/domesticLocation/detail/1560">
        ขอบคุณข้อมูลอ้างอิงจาก
      </a></small
    >
  </p>
</template>
<style scoped>
</style>
