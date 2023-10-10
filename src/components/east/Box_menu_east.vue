<template>
  <!-- แถบ Menu  -->
  <div class="NavBar">
    <nav class="NavMenu">
      <router-link
        :to="{ name: 'home_east' }"
        class="itemNav"
        style="border-radius: 30px"
        >หน้าแรก</router-link
      >
      <router-link
        :to="{ name: 'page_product_east' }"
        class="itemNav"
        style="border-radius: 30px"
        >สินค้าแนะนำ</router-link
      >
      <router-link
        :to="{ name: 'place_01_east' }"
        class="itemNav"
        style="border-radius: 30px"
        >เกาะสีชัง</router-link
      >
      <router-link
        :to="{ name: 'place_02_east' }"
        class="itemNav"
        style="border-radius: 30px"
        >วัดมณีวงศ์
      </router-link>
      <router-link
        :to="{ name: 'place_03_east' }"
        class="itemNav"
        style="border-radius: 30px"
        >วัดหงษ์ทอง
      </router-link>
      <router-link
        :to="{ name: 'place_04_east' }"
        class="itemNav"
        style="border-radius: 30px"
        >วัดถ้ำเขาประทุน</router-link
      >
      <router-link
        :to="{ name: 'place_05_east' }"
        class="itemNav"
        style="border-radius: 30px"
        >ถ้ำน้ำเขาศิวะ
      </router-link>
    </nav>
  </div>
</template>
<style scoped>
.NavBar{
  background-color: #176B87;
  padding: 10px;
  padding-inline: 110px;
  margin-bottom: 15px;
}
.NavMenu{
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
}
.itemNav{
  border: 2px solid white;
  border-radius: 16px;
  padding-block: 10px;
  padding-inline: 20px;
  color: white;
  text-decoration: none;
  background-color: #004858;
}
.itemNav:hover{
  border: 2px solid rgba(65, 3, 3, 0.274);
  background-color: rgba(0, 0, 0, 0.144);
  border-radius: 16px;
  padding-block: 10px;
  padding-inline: 20px;
  color: white;
  text-decoration: none;
}
</style>