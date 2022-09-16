<script setup lang="ts">
// (function reverseWords(str: string): string {
//   return str
//     .split(" ")
//     .map((word) => word.split("").reverse().join(""))
//     .join(" ");
// })("hello world!");

// (function printerError(s: string): string {
//   let letters = "abcdefghijklm";
//   let errors = 0;
//   for (let i = 0; i < s.length; i++) {
//     if (!letters.includes(s[i])) {
//       errors++;
//     }
//   }
//   return `${errors}/${s.length}`;
// })("aaaaaaaaaaaaaaaabbbbbbbbbbbbbbbbbbmmmmmmmmmmmmmmmmmmmxyz");

// (function wave(str: string): Array<string> {
//   let finalArray = [];
//   for (let index = 0; index < str.length; index++) {
//     let letterArray = str.split("");
//     for (let j = 0; j < letterArray.length; j++) {
//       if (index == j) {
//         letterArray[j] = letterArray[j].toUpperCase();
//         console.log(letterArray[j]);
//       }
//     }
//     letterArray[index] == " " ? "" : finalArray.push(letterArray.join(""));
//   }

//   return finalArray;
// })("two words");

// (function twoOldestAges(ages: number[]): number[] {
//   let sortedArray: any = ages.sort((a, b) => a - b);
//   console.log([sortedArray.at(-2), sortedArray.at(-1)]);

//   return [];
// })([1, 5, 87, 45, 8, 8]);
</script>
<template>
  <div>
    <h1>Kata 3</h1>
  </div>
</template>
