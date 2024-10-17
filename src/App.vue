<script setup lang="ts">
import { ref } from 'vue';
import Bt2 from './Session7/bt2.vue';
import Bt3 from './Session7/bt3.vue';
import Bt5 from './Session7/bt5.vue';
import Bt6 from './Session7/bt6.vue';


// let userlist = [{id: 1, name: "Nguyễn Thanh Hạ", price: 0, quantity: 0 }]

function handleClick() {
  alert('Bạn đã nhấn vào nút Xem chi tiết');
}
</script>
<template>
  <div>
    <!-- <Bt2 :userList="userlist">

    </Bt2> -->

    <!-- <Bt3>
      <p>Count: {{ count }}</p>
    <CountChildren @increment="incrementCount" />
    </Bt3> -->

    <!-- <Bt5>
      <h3>Thông báo từ hệ thống</h3>
      <p>Đây là nội dung của modal. Bạn có thể đóng modal bằng cách nhấn vào nút 'Close'.</p>
    </Bt5> -->

    <Bt6>
      <Card>
    <template #header>
      <h3>Thông tin sản phẩm</h3>
    </template>

    <template #body>
      <p>Đây là mô tả ngắn gọn về sản phẩm này. Sản phẩm có các tính năng nổi bật và giá cả hợp lý.</p>
    </template>

    <template #footer>
      <button @click="handleClick">Xem chi tiết</button>
    </template>
  </Card>
    </Bt6>
  </div>
</template>


<style scoped>

</style>
