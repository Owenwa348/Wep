<script setup>
import Header_box_east from '../east/Box_menu_east.vue'
import { ref } from 'vue'
import { Otop_eastStore } from '../../stores/All_product'

const otop_eastStore = Otop_eastStore()
const otop_east_all = ref(otop_eastStore.Otop_east_list)
</script>

<template>
  <!-- แถบ ภาพ  -->

  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-image-container">
        <img
          src="https://images.wallpaperscraft.com/image/single/girl_smile_beret_1053550_1920x1080.jpg"
          class="d-block w-100"
          alt="..."
          height="450"
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
        <h1 class="display-3">สินค้าภาคตะวันออก</h1>
        <h5 class="h4">First slide label</h5>
        <p class="h4">Some representative placeholder content for the first slide.</p>
      </div>
    </div>
  </div>

  <!-- แถบ menu -->
  <Header_box_east></Header_box_east>

  <!--กิจกรรมที่น่าสนใจ-->
  <div class="container">
    <h1 class="textcenter"><strong>กิจกรรมที่น่าสนใจ</strong></h1>
    <hr />

    <div class="row row-cols-1 row-cols-md-2 g-4">
<<<<<<< HEAD
      <div class="col" v-for="(i,index) in otop_east_all" :key="index">
        <div class="d-flex flex-column flex-lg-row gap-3 align-items-start align-items-lg-center py-3 link-body-emphasis text-decoration-none border-top">
          <img :src="i.img"
          class="rounded float-start" alt="..." width="300" height="300"
          />
          <div class="card-body">
            <h5 class="card-text mb-auto"><strong class="h3">{{ i.name }}</strong></h5>
            <p class="card-text"><strong>ประเภท: {{ i.category }}</strong></p>
            <p class="card-text"><strong>ราคา:{{ i.price }} บาท</strong></p>
            <p class="card-text">{{ i.text }} </p>
            <button type="button" class="btn btn-dark" style="border-radius: 30px">ลงตะกร้า</button>
=======
      <div class="col" v-for="(i, index) in otop_east_all" :key="index">
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
>>>>>>> 42d26833cd833e5d8ce5b5a48bf943d8b259fb91
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.textcenter{
  text-align: center;
  margin-inline: 420px;
  border-bottom: 2px solid;
}
</style>
