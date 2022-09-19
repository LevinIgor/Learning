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

// solution(10);

// function firstNonConsecutive(arr: number[]) {
//   for (let index = 0; index < arr.length - 1; index++) {
//     if (arr[index] + 1 !== arr[index + 1]) {
//       return arr[index + 1];
//     }
//   }
// }
// console.log(firstNonConsecutive([1, 2, 3, 4, 6, 7, 8]));

// function getLengthOfMissingArray(arrayOfArrays: any[]) {
//   let sortedArrayArrays = arrayOfArrays.sort((a, b) => a.length - b.length);
//   let temp = 0;
//   let answer = 0;
//   console.log(sortedArrayArrays);
//   if (sortedArrayArrays.length == 0 || sortedArrayArrays[0].length == 0) {
//     return 0;
//   }
//   sortedArrayArrays.forEach((element) => {
//     if (temp + 1 != element.length) {
//       answer = temp + 1;
//     }
//     temp = element.length;
//   });
//   return answer;
// }
// console.log(getLengthOfMissingArray([]));

// const towerBuilder = (nFloors: number) => {
//   let arr = [];
//   let padding = nFloors - 1;
//   for (let index = 0; index < nFloors; index++) {
//     let _arr = "";
//     for (let j = 1; j < nFloors * 2; j++) {
//       if (j > padding && j < nFloors * 2 - padding) {
//         console.log(j > padding, j < nFloors * 2 - padding);
//         _arr += "*";
//       } else {
//         _arr += "";
//       }
//     }
//     padding--;
//     arr.push(_arr);
//   }

//   return arr;
// };
// console.log(towerBuilder(3));

// function decipherThis(str: string) {
//   let arrayWords: any = str.split(" ");
//   let arrayWithoutUnicode: any = [];
//   arrayWords.forEach((word: string) => {
//     let code = "";
//     let _word = "";
//     word.split("").forEach((letter) => {
//       if (Number.isInteger(+letter)) {
//         code += letter;
//       } else {
//         _word += letter;
//       }
//     });
//     arrayWithoutUnicode.push(`${String.fromCharCode(+code)}${_word}`);
//   });
//   arrayWithoutUnicode.forEach((word: any, index: number) => {
//     let letter = word[1];
//     word = word.split("");
//     word[1] = word.at(-1);
//     word[word.length - 1] = letter;
//     word = word.join("");
//     arrayWithoutUnicode[index] = word;
//   });
//   return arrayWithoutUnicode.join(" ");
// }
// console.log(
//   decipherThis("72eva 97 103o 97t 116sih 97dn 115ee 104wo 121uo 100o")
// );

// function humanReadable(seconds: number) {
//   let second: any = 0;
//   let hours: any = 0;
//   let minute: any = 0;
//   for (let index = 0; index < seconds; index++) {
//     second++;
//     if (second == 60) {
//       minute++;
//       second = 0;
//     }
//     if (minute == 60) {
//       hours++;
//       minute = 0;
//     }
//   }

//   return formateTime(hours, minute, second).join(":");
// }
// function formateTime(...arg: number[]) {
//   arg.forEach((date: any, index) => {
//     if (date < 10) {
//       date = "0" + date.toString();
//     }
//     arg[index] = date;
//   });
//   return arg;
// }
// console.log(humanReadable(60));
</script>
<template>
  <h1>Kata 4</h1>
</template>
