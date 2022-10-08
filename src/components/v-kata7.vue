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

// function solve(s: string) {
//   return s.match(/[qwe]/gi);
// }
// console.log(solve("qeerqq"));

// function specialNumber(n: number) {
//   return n.toString().match(/[012345]/g)?.length === n.toString().length
//     ? "Special"
//     : "NOT!!";
// }
// console.log(specialNumber(1234));

// let str = "slkfweof43";

// console.log(str.matchAll(/[1]/g));

// function shuffledArray(shuffled: number[]): number[] {
//   let sum = shuffled.reduce((a, b) => a + b) / 2;
//   let res: number[] = [];
//   shuffled.forEach((el) => {
//     if (el != sum) {
//       res.push(el);
//     } else {
//       sum = Infinity;
//     }
//   });
//   return res.sort((a, b) => a - b);
// }

// console.log(shuffledArray([-3, -3]));

//  function vowelIndices(word: string): number[] {
//   let arr: number[] = [];
//   let vowels = ["e", "y", "u", "o", "i", "a"];
//   word
//     .split("")
//     .map((letter, index) =>
//       vowels.includes(letter) ? arr.push(index + 1) : ""
//     );
//   return arr;
// }

// var uniqueInOrder = function (iterable: any) {
//   let res = [];
//   for (let i = 0; i < iterable.length; i++) {
//     if (iterable[i] !== iterable[i + 1] || iterable[i + 1] === undefined) {
//       res.push(iterable[i]);
//     }
//     console.log(iterable[i]);
//   }
//   return res;
// };
// console.log(uniqueInOrder("AAAABBBCCDAABBB"));

// function longestRepetition(text: string): [string, number] {
//   let unique = [...new Set(text.split(""))];
//   let maxCount = { letter: "", count: 0 };
//   for (let i = 0; i < unique.length; i++) {
//     let count = 0;
//     for (let j = i; j < text.length; j++) {
//       if (unique[i] === text[j]) {
//         count += 1;
//       } else {
//         if (maxCount.count < count) {
//           maxCount.count = count;
//           maxCount.letter = text[i];
//           console.log(count);
//           count = 0;
//         }
//       }
//     }
//   }
//   return [maxCount.letter, maxCount.count];
// }

// console.log(longestRepetition("abbbbb"));

//  function findOutlier(integers: number[]): number {
//   return Math.min(
//     integers.filter((n) => n % 2 == 0).length,
//     integers.filter((n) => n % 2 !== 0).length
//   );
// }
// function orderedCount(text: string): any {
//   let unique = [...new Set(text.split(""))];
//   console.log(unique);
//   let result: [string, number][] = [];
//   for (let i = 0; i < unique.length; i++) {
//     let temp: [string, number] = [unique[i], 0];
//     console.log(temp);
//     for (let j = 0; j < text.length; j++) {
//       if (unique[i] === text[j]) {
//         temp[1] += 1;
//       }
//     }
//     result.push(temp);
//   }
//   return result;
// }

// console.log(orderedCount("aabbcca"));

// function sumOfDifferences(arr: number[]): number {
//   let sorted = arr.sort((a, b) => b - a);

//   return sorted.reduce((acc, number, index) => {
//     if (index == sorted.length - 1) return acc;
//     return acc + (number - sorted[index + 1]);
//   }, 0);
// }
// console.log(sumOfDifferences([1, 2, 10]));
// function mean(lst: string[]): [any, string] {
//   let numbersSum: any = lst
//     .toString()
//     .match(/[0-9]/g)?.map((el) => Number(el))
//     .reduce((a, b) => a + b);
//   console.log(numbersSum);
//   let letters: any = lst.toString().match(/[a-z]/gi);
//   return [numbersSum / 10, letters.join("")];
// }
// console.log(
//   mean([
//     "u","6","d","1","i","w","6",
//     "s",
//     "t",
//     "4",
//     "a",
//     "6",
//     "g",
//     "1",
//     "2",
//     "w",
//     "8",
//     "o",
//     "2",
//     "0",
//   ])
// );

function gematria(str: string): number {
  let values: any = {
    a: 1,
    b: 2,
    c: 3,
    d: 4,
    e: 5,
    f: 6,
    g: 7,
    h: 8,
    i: 9,
    k: 10,
    l: 20,
    m: 30,
    n: 40,
    o: 50,
    p: 60,
    q: 70,
    r: 80,
    s: 90,
    t: 100,
    u: 200,
    x: 300,
    y: 400,
    z: 500,
    j: 600,
    v: 700,
    w: 900,
  };
  let sum = 0;
  str = str.replace(/ /g, "");
  for (let i = 0; i < str.length; i++) {
    sum += values[str[i].toLowerCase()];
    console.log(str[i]);
  }
  return sum;
}
console.log(gematria("Coding is fun"));
</script>
<template><h1>Kata 7</h1></template>
