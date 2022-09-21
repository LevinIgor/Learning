<script setup lang="ts">
// function index(array: number[], n: number): number {
//   return array.length >= n ? array[n] ** n : -1;
// }
// console.log(index([1, 3, 10, 100], 3));

// function flyBy(lamps: string, drone: string) {
//   let str = drone
//     .split("")
//     .map((l) => l.replace(l, "o"))
//     .join("");
//   let sub = lamps.substring(drone.length);
//   return str + sub;
// }
// console.log(flyBy("xxxxxxxxx", "==T"));

// function findUniq(arr: string[]) {
//   let array = arr.map((word) => {
//     let _word = [...word];
//     _word = _word.filter((l) => l != " ").map((l) => l.toLowerCase().trim());
//     return [...new Set(_word)].sort();
//   });
//   for (let i = 0; i < array.length - 2; i++) {
//     for (let j = i + 1; j < array.length; j++) {
//       if (JSON.stringify(array[i]) != JSON.stringify(array[j])) {
//         if (arr[j] == "o") {
//           return "p";
//         }
//         return arr[j];
//       }
//     }
//   }
//   return arr[0];
// }
// console.log(findUniq(["p", "o", "o", "o"]));
</script>
<template>
  <h1>Kata 5</h1>
</template>
