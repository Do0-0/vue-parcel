<template>
  <div class="hello-world">
    <h1>Hello World!</h1>
  </div>
</template>

<script>
import TU from 'datetime-util'
export default {
  name: 'hello-world',
  mounted() {
  	// let timeString = TU.calculateTime(new Date(), 'D', 2);
  	let timeString = TU.formatTime(new Date(), 'yyyy年MM月dd日 HH时mm分ss秒');
  	console.info(timeString)
  }
}
</script>