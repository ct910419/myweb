<template>
  <div>
	<div class="bg">
    <img src="../assets/bg.png" alt="bg">
  </div>
	<div id="game">
    <pre> FUNNY</pre>
  </div>
	<vue-p5 class="fun"
        @preload="preload"
        @setup="setup"
        @draw="draw"
        @keypressed="keyPressed"
        @mousemoved="mouseMoved"
        @mousedragged="mouseDragged">
  </vue-p5>
  </div>
</template>

<style>
.bg{
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  z-index: -999;
}
.bg img{
  min-height: 100%;
  width: 100%;
}
#game{
  font-family:Arial, Helvetica, sans-serif;
  position: relative;
  top: 95px;
  text-align: center;
  font-size: 72px;
  letter-spacing: 195px;
  color:#DAD7CD;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
}
.fun{
	position: absolute;
	float: left;
	left: 0;
	bottom: 0;
	margin: 0;
	padding: 0;
	z-index: -500;
	top: 350px;
}
</style>

<script>
import VueP5 from "vue-p5";
export default {
  name: "p5-example",
  components: {
    "vue-p5": VueP5
  },
  data: () => ({
    max_distance: 0,
    t: 0,
  }),
  methods: {
    setup(sketch) {
      sketch.createCanvas(1500, 1050);
      sketch.noStroke();
			sketch.fill(163, 177, 138)
    },
    draw(sketch) {
      sketch.background(218, 215, 205);

      for (let x = 0; x <= sketch.width; x += 30) {
    		for (let y = 0; y <=sketch.height; y += 30) {
          const xAngle = sketch.map(sketch.mouseX, 0, sketch.width, -4 * sketch.PI, 4 * sketch.PI, true);
          const yAngle = sketch.map(sketch.mouseY, 0, sketch.height, -4 * sketch.PI, 4 * sketch.PI, true);
          const angle = xAngle * (x / sketch.width) + yAngle * (y / sketch.height);
          const myX = x + 20 * sketch.cos(2 * sketch.PI * this.t + angle);
          const myY = y + 20 * sketch.sin(2 * sketch.PI * this.t + angle);
          sketch.ellipse(myX, myY, 10); // 绘制粒子
    		}
      }
      this.t = this.t + 0.01; // 更新时间
    },
  }
};
</script>

