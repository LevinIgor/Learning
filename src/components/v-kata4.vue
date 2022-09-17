<script setup lang="ts">
// function digitalRoot(n: number): any {
//   let final = n
//     .toString()
//     .split("")
//     .map((a) => Number(a))
//     .reduce((total, current) => (total += current));
//   return final > 9 ? digitalRoot(final) : final;
// }
// console.log(digitalRoot(456));

//  function abbrevName(name: string): string {
//     return name.split(' ').map((part)=> part[0].toUpperCase()).join('.')
// }

//  function number(array: string[]): string[]{
//   return array.map((el, i) => `${i+1}: ${el}`);
// }

// (function findUniq(arr: number[]): number {
//   let numbers = Array.from(new Set(arr));
//   let count = arr.filter((number) => number == numbers[0]).length;

//   return count > 1 ? numbers[1] : numbers[0];
// })([1, 1, 1, 2, 1, 1]);

// function solution(number: number) {
//   let array = [];
//   for (let index = 0; index < number; index++) {
//     if (index % 3 == 0 || index % 5 == 0) {
//       array.push(index);
//     }
//   }

//   return array.reduce((a, b) => a + b, 0);
// }

solution(10);
</script>
<template>
  <h1>Kata 4</h1>
</template>
