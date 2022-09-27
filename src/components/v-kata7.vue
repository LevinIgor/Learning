<script setup lang="ts">
// let number: any = 12233;
// number = [...String(number)].map((number) => +number);
// let res = 0;
// for (let index = 1; index <= Math.max(...number); index++) {
//   let count = number.filter((number: number) => number == index).length;
//   index == count ? (res = count) : null;
// }
// console.log(res);

// function sumPairs(ints: number[], s: number) {
//   let res = { first: 0, second: 0, index: Infinity };
//   let memo: any = [];
//   for (let i = 0; i < ints.length - 1; i++) {
//     if (memo.includes(ints[i])) {
//       continue;
//     }
//     for (let j = i + 1; j < ints.length; j++) {
//       if (ints[i] + ints[j] == s && j < res.index) {
//         res = { first: ints[i], second: ints[j], index: j };
//       }
//     }
//     memo.push(ints[i]);
//   }
//   return res.index == Infinity ? undefined : [res.first, res.second];
// }

// class Test {
//   x = 1;
//   f() {
//     console.log(this.x);
//   }
// }
// let test = new Test();
// console.log(test.f());

// function balancedNum(number: number): string {
//   let length = number.toString().length;
//   let res = "";
//   if ((length & 1) === 0) {
//     let left: any = number.toString().slice(0, length / 2 - 1);
//     let right: any = number.toString().slice(-length / 2 + 1);

//     console.log(left, right);
//     left = [...left].reduce((acc, numb) => (acc += +numb), 0);
//     right = [...right].reduce((acc, numb) => (acc += +numb), 0);
//     res = left === right ? "Balanced" : "Not Balanced";
//   } else {
//     let left: any = number.toString().slice(0, Math.floor(length / 2));
//     let right: any = number.toString().slice(-Math.ceil(length / 2) + 1);
//     left = [...left].reduce((acc, numb) => (acc += +numb), 0);
//     right = [...right].reduce((acc, numb) => (acc += +numb), 0);
//     res = left === right ? "Balanced" : "Not Balanced";
//   }
//   return res;
// }

// console.log(balancedNum(56239814));

// let str = "qwe0rt";
// let length = str.length;
// let res =
//   (length & 1) === 0
//     ? str.slice(Math.floor(length / 2) - 1, Math.ceil(length / 2) + 1)
//     : str.slice(Math.floor(length / 2), Math.ceil(length / 2));
// console.log(res);
</script>
<template><h1>Kata 7</h1></template>
