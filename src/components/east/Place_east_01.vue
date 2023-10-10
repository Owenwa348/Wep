<template>
  <!-- แถบ ภาพ  -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-image-container">
        <img
          src="https://www.hellosummer.60เส้นทางความสุข.com/wp-content/uploads/2020/02/%E0%B9%80%E0%B8%81%E0%B8%B2%E0%B8%B0%E0%B8%AA%E0%B8%B5%E0%B8%8A%E0%B8%B1%E0%B8%87-Banner.jpg"
          class="d-block w-100"
          alt="..."
          :height="'450'"
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
        <h5 class="display-3">เกาะสีชัง</h5>
        <p class="h4">เกาะสีชัง อ.เกาะสีชัง จ.ชลบุรี</p>
      </div>
    </div>
  </div>

  <!-- แถบ menu -->
  <Header_box_east></Header_box_east>

  <!-- แถบ เนื้อหา -->

  <!-- box รูปซ้าย -->
  <div class="container">
    <div class="card mb-3" style="max-width: 1500px">
      <div class="row g-0">
        <div class="col-md-4">
          <img
            src="https://img.kapook.com/u/2019/sutasinee/03/k2.jpg"
            class="img-fluid rounded-start"
            alt="..."
          />
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="h2"><strong>เกาะสีชัง</strong></h5>
            <p class="h5">
              บุคคลที่มีหัวใจอนุรักษ์ เกาะสีชังถือเป็นจุดหมายที่น่าสนใจ
              ด้วยความอันซีนของจุดชมวิวที่มีให้เลือกสร้างซีนโรแมนติกได้ถึง 5 พื้นที่ เช่น
              ปลายแหลมถ้ำพัง, เสาธงอัษฎางค์, สะพานอัษฎางค์, ช่องอิสริยาภรณ์ และทะเลแหวกท้ายเกาะ
              ไม่ว่าจะอยากชมพระอาทิตย์ขึ้นหรือตกก็มีจุดชมวิวอยู่มากมาย
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
            <p class="h5">
              นอกจากนี้ ตัวเกาะยังมีคอนเซปต์น่ารักในการจัดการกับสิ่งแวดล้อม
              ทั้งการนำขยะบนเกาะไปทำปุ๋ย การปลูกปะการังอ่อน การเปิดธนาคารปูและสัตว์น้ำหายาก
              เพื่อเป็นการอนุรักษ์ทรัพยากรทางทะเลรอบๆ เกาะให้มีความยั่งยืน ใครรู้ตัวว่าเป็นสาย ECO
              กดจองที่พักบนเกาะได้เลย โดยท่องเที่ยวได้ตลอดทั้งปี
            </p>
          </div>
        </div>
        <div class="col-md-4">
          <img
            src="https://roijang.com/wp-content/uploads/2022/07/aerial-view-wood-waterfront-pavilion-koh-si-chang-island-thailand-asdang-bridge-1.jpg"
            class="img-fluid rounded-start"
            alt="..."
          />
        </div>
      </div>
    </div>

    <!-- สิ่งของแนะนำขาย -->
    <h1 class="textcenter"><strong>แนะนำสินค้า</strong></h1>
    <hr />

    <div class="row row-cols-1 row-cols-md-2 g-4">
<<<<<<< HEAD
      <div class="col" v-for="index in 4" :key="index">
        <div class="d-flex flex-column flex-lg-row gap-3 align-items-start align-items-lg-center py-3 link-body-emphasis text-decoration-none border-top">
          <img
            src="https://media.discordapp.net/attachments/1153766321666932836/1153887346882773063/1.jpg?ex=65178e55&is=65163cd5&hm=3000ed1d1b278ba7d013ff4a926d2caca1902c2b30928485f6b0d1e897429086&=&width=585&height=585"
            class="rounded float-start" alt="..." width="300" height="300"
          />
          <div class="card-body">
            <h5 class="card-title">Card title</h5>
            <p class="card-text">
              This is a longer card with supporting text below as a natural lead-in to additional
              content. This content is a little bit longer.
            </p>
            <button type="button" class="btn btn-dark" style="border-radius: 30px">LINK สินค้า</button>
=======
      <div
        class="card mb-3"
        style="max-width: 1500px"
        v-for="(i, index) in item_advice_east_01_all"
        :key="index"
      >
        <div class="row g-0">
          <div class="col-md-4">
            <img :src="i.img" class="img-fluid rounded-start" alt="..." />
          </div>
          <div class="col-md-8">
            <div class="card-body">
              <h5 class="card-title">{{ i.name }}</h5>
              <p class="card-text">{{ i.category }}</p>
            </div>
>>>>>>> 42d26833cd833e5d8ce5b5a48bf943d8b259fb91
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
<style scoped>
.textcenter{
  text-align: center;
  margin-inline: 500px;
  border-bottom: 2px solid;
}
</style>
<script setup>
import Header_box_east from '../east/Box_menu_east.vue'

import { ref } from 'vue'
import { item_advice_east_01Store } from '../east/index_east'

const item_advice_east_01 = item_advice_east_01Store()
const item_advice_east_01_all = ref(item_advice_east_01.item_advice_east_list_01)
</script>
