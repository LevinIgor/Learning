<script setup lang="ts">
function makeAdder(x: any) {
  return function (y: any) {
    return x + y;
  };
}
var add5 = makeAdder(10);
var add10 = makeAdder(100);

console.log(add5(2)); // 12
console.log(add10(2)); // 102
</script>
