<script setup lang="ts">
function highAndLow(numbers: string) {
  let arr = numbers.split(" ").map(Number);
  return `${Math.max(...arr)} ${Math.min(...arr)}`;
}
console.log(highAndLow("1 2 3 4 5"));
</script>
