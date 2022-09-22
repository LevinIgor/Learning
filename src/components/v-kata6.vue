<script setup lang="ts">
// function countPositivesSumNegatives(input: any) {
//   if (input.length == 0) {
//     return [];
//   }
//   if (input.includes(null)) {
//     return input;
//   }
//   let count = input.reduce((_count: any, element: any) =>
//     element > 0 ? (_count += 1) : _count
//   );
//   let sum = input.reduce((_sum: any, element: any) =>
//     element < 0 ? (_sum += element) : _sum
//   );
//   return [count, sum];
// }
// console.log(
//   countPositivesSumNegatives([
//     0, 2, 3, 0, 5, 6, 7, 8, 9, 10, -11, -12, -13, -14,
//   ])
// );

// let arr = [
//   { name: "Nick", id: 0, age: 10 },
//   { name: "Alex", id: 1, age: 20 },
//   { name: "Moly", id: 2, age: 30 },
// ];

// function getKeyFromArray(arr: Array<object>, key: string) {
//   return arr.map((item: any) => {
//     return { key: item[key] };
//   });
// }

// console.log(getKeyFromArray(arr, "name"));

// function isDivisible(n: number, x: number, y: number) {
//   if (x * y > n) {
//     return false;
//   }
//   if (x * y == n) return true;
//   if (n % (x * y) == 0) return true;
//   return false;
// }
// console.log(isDivisible(50, 4, 3));

// function countSheep(num: number): string {
//   let str = "";
//   for (let index = 1; index <= num; index++) {
//     str += `${index} sheep...`;
//   }
//   return str; // your code here
// }
// console.log(countSheep(2));

// function generateShape(int: number): string {
//   let first = "+".repeat(int);
//   let second = `${first}/n`.repeat(int);
//   return second.slice(0, -2);
// }
// console.log(generateShape(1));

// console.log(
//   "192145678"
//     .split("")
//     .map((e) => parseInt(e))
//     .sort((a, b) => a - b).join('')
// );

// function houseNumbersSum(inputArray: number[]) {
//   return [...inputArray.slice(0, inputArray.indexOf(0))].reduce(
//     (box, item) => (box += item),
//     0
//   );
// }
// console.log(houseNumbersSum([1, 2, 3, 4, 5, 0]));

function maxMultiple(divisor: number, bound: number): number {
  let maximum = divisor;
  while (maximum <= bound) {
    maximum = maximum * 2;
    console.log(maximum);
  }
  return maximum/2;
}
console.log(maxMultiple(2, 7));
</script>
<template>
  <h1>Kata 6</h1>
</template>
