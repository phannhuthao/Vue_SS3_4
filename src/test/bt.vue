<template>
    <!-- <img :src="urlImg" alt="" width="400px" height="200px">
  <br>
  <h1 :class="test ? 'test': ''">Nhìn cái gì</h1>

  <button v-on:click="testColor(5)">Change Color</button>
  <br>
  <input @keydown.enter="EnterKey" type="text"><br>

  <span>Tên của user {{ user.name }}</span><br>

  <span>Gia trị là: {{ numberTinhTong }}</span>
  <button @click="()=> {
    number = number + 1
  }" >Tăng giá trị</button>

  <h1 v-on:click="() => {
    count++
  }" >Giá của count là: {{ count }}</h1> -->
</template>

<script setup lang="ts">
// let urlImg = "https://huanluyencho119.vn/storage/9c/b8/9cb8sza53kwquhgx4wmgnll6g3wu_cach-huan-luyen-cho-phat-mot-chu-cho-khi-lam-sai-lieu-co-hieu-qua-nhu-mong-doi.jpg"
// // let test:boolean = true;
// let test = ref(false);

// let user = {
//   id: 1,
//   name: "Hào",
//  }

 
// let count = ref(0);

//  watch(count, (giaTriCountMoi, giaTriCountTruocDo, ) => {
//   console.log("Giá trị count trước đó là: ", giaTriCountTruocDo);
//   console.log("Giá trị count mới", giaTriCountMoi)
//  })

// function testColor(a: number) {
//   console.log("Đã vào",a)
//   test.value = !test.value

//   console.log("Giá trị Test", test)
// }

// function EnterKey() {
//   console.log("Enter key");
// }

// let number = ref(1);

// let numberTinhTong = computed(() => {
//   return number.value + 100;
// })
</script>

<style scoped>
/* .test {
  color: red
} */
</style>