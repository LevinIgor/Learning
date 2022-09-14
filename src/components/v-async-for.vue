<script setup lang="ts">
// for (let i = 0; i < 10; i++) {
//   setTimeout(() => {
//     console.log(i);
//   }, 1000 + i * 1000);
// }

for (var i = 0; i < 10; i++) {
  setTimeout(() => {
    console.log(i); // 10
  }, 3000);
}

for (let i = 0; i < 10; i++) {
  setTimeout(() => {
    console.log(i); // 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
  }, 3000);
}


</script>
<template>
  <div class="async">
    <h1>Async For</h1>
  </div>
</template>
<style scoped>

</style>
