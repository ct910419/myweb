<template>
<div>
  <div class="bg">
    <img src="../assets/bg.png" alt="bg">
  </div>
  <div>
  <router-link to="/about" class="wrap bouncingLoader">
  CT
  </router-link>
  </div>
  <div id="footer">
		<pre>



		</pre>
	</div>
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
.wrap {
  background: url("https://convertingcolors.com/gradient-A3B18A.svg") no-repeat left bottom;
  background-size: cover;
  font-size: 600px;
  text-align: center;
  padding: 50px;
  font-weight: bold;
  color: transparent;
  box-shadow:  4px 4px 2px rgba(0, 0, 0, 0.30);
  -webkit-background-clip: text;
  background-clip: text;
  position: relative;
  top: 100px;

  display: inline-block;
  margin: 0 0.5rem;

  animation: bounceIn; /* referring directly to the animation's @keyframe declaration */
  animation-duration: 2s; /* don't forget to set a duration! */
}
.bouncingLoader > div, .bouncingLoader:before, .bouncingLoader:after {
    display: inline-block;
    width: 30px;
    height: 30px;
    margin-bottom: -5px;
    border-radius: 50%;
    animation: bouncing-loader 0.6s infinite alternate;
    background: url("https://www.colorhexa.com/a3b18a.png") no-repeat left bottom;
    background-size: cover;
}

.bouncingLoader > div, .bouncingLoader:before, .bouncingLoader:after {
    content: "";
}

.bouncingLoader > div {
    margin: 0 5px;
}

.bouncingLoader > div {
    animation-delay: 0.2s;
}

.bouncingLoader:after {
    animation-delay: 0.4s;
}

@keyframes bouncing-loader {
    to {
        opacity: 0.1;
        transform: translate3d(0, -16px, 0);
    }
}
#footer{
	background-color: #dad7cd00;
	position: relative;
	width: 80%;
	top: 100px;
	margin: 0;
	padding: 0;
	float: center;
	left: 100px;
}
</style>

