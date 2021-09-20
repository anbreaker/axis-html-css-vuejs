<template>
  <div class="chart">
    <div class="tick" v-for="iX in 11" :key="iX">
      <span>{{ iX * 100 - 100 }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Axis"
};
</script>

<style scoped>
.chart {
  width: 95vw;
  height: 400px;
  margin: 20px 10px 50px 10px;
  position: relative;
  border-left: 2px solid black;
  /* border: 1px solid crimson; */
}

.chart:after {
  content: " ";
  display: block;
  position: relative;
  border: 1px solid black;
  top: 400px;
  left: -2px;
}

.tick {
  border-left: 2px solid black;
  height: 18px;
  top: 400px;
  position: absolute;
}

.tick:nth-child(1) {
  left: -2px;
}

.tick:nth-child(2) {
  left: calc(95vw / 10);
}

.tick:nth-child(3) {
  left: calc(95vw / 10 * 2);
}

.tick:nth-child(4) {
  left: calc(95vw / 10 * 3);
}

.tick:nth-child(5) {
  left: calc(95vw / 10 * 4);
}

.tick:nth-child(6) {
  left: calc(95vw / 10 * 5);
}

.tick:nth-child(7) {
  left: calc(95vw / 10 * 6);
}

.tick:nth-child(8) {
  left: calc(95vw / 10 * 7);
}

.tick:nth-child(9) {
  left: calc(95vw / 10 * 8);
}

.tick:nth-child(10) {
  left: calc(95vw / 10 * 9);
}

.tick:nth-child(11) {
  left: calc(95vw);
}

.tick:nth-child(5n + 1) {
  border-left: 4px solid darkred;
  height: 24px;
}

.tick > span {
  position: relative;
  width: 10px;
  left: -5px;
  top: 26px;
}

.tick:nth-child(3n + 1) > span {
  left: -6px;
  font-weight: bold;
}
</style>
