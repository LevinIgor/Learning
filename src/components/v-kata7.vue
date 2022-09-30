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

// let values = [-2, -4, -6, -11, -11, -5, -3];
// let sortArray = values.sort((a, b) => a - b);
// let middle = sortArray[0];
// sortArray = sortArray.slice(1);
// let leftArray = sortArray.filter((_, index) => index & 1);
// let rightArray = sortArray.filter((_, index) => !(index & 1));
// leftArray = leftArray.reverse();
// console.log([...leftArray, middle, ...rightArray]);

// let array = [9,8,7,6,5,4,3,2];
// let min = 0;

// for (let i = 0; i < array.length - 1; i++) {
//   min = array[i];
//   for (let j = i + 1; j < array.length; j++) {
//     if (array[j] < min) {
//       min = array[j];
//       let temp = array[i];
//       array[i] = array[j];
//       array[j] = temp;
//     }
//   }
// }
// console.log(array);
//  const mutate = (chromosome: string, p: number): string => {
//   if(p == 0) return chromosome
//   if(p == 1){
//     return chromosome.split('').map((el)=> el == '1' ? 0:1).join('')
//   }
//   return chromosome.split('').map(()=>'1').join('')

// };

// function sumCubes(n: number): any {
//   return n > 0 ? n ** 3 + sumCubes(n - 1) : 0;
// }

// console.log(sumCubes(3));

// function rowWeights(arr: number[]) {
//   return arr.reduce(
//     (acc: number[], number, index) =>
//       index & 1 ? acc.push(number) : acc.push(number),
//     [0,0]
//   );
// }
// console.log(rowWeights([1, 2, 3, 4, 5, 6, 7, 8]));
</script>
<template><h1>Kata 7</h1></template>
