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
	top: 70px;
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
  }),
  methods: {
    setup(sketch) {
      sketch.createCanvas(1500, 1050);
      sketch.noStroke();
			this.max_distance = sketch.dist(0, 0, sketch.width, sketch.height);
    },
    draw(sketch) {
      sketch.background(163, 177, 138);

      for (let i = 0; i <= sketch.width; i += 20) {
    		for (let j = 0; j <=sketch.height; j += 20) {
      		let size = sketch.dist(sketch.mouseX, sketch.mouseY, i, j);
					size = (size / this.max_distance) * 25;
					sketch.fill(218, 215, 205);
      		sketch.ellipse(i, j, size, size);
    		}
  		}
    },
  }
};
</script>

