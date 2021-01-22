<template>
<div>
	<div class="bg">
    <img src="../assets/bg.png" alt="bg">
  </div>
	<div id="profile">
    <pre> PROFILE</pre>
  </div>
  <div class="op">
    <el-tabs v-model="activeName" @tab-click="handleClick">
    <el-tab-pane label="海報美學" name="first">
      <div class="p">
        <pre id="pt1"> 練習分析海報</pre>
        <img src="../assets/p1.jpg" alt="p1" width="400px" height="300px">
        <img src="../assets/p2.jpg" alt="p2" width="400px" height="300px">
        <img src="../assets/p3.jpg" alt="p3" width="400px" height="300px">
        <img src="../assets/p4.jpg" alt="p4" width="400px" height="300px">
        <pre id="pt2"> 為上一堂課製作書封</pre>
        <img id="p5" src="../assets/p5.jpg" alt="p5" width="300px" height="400px">
        <img id="p5" src="../assets/p6.jpg" alt="p6" width="300px" height="400px">
      </div>
    </el-tab-pane>
    <el-tab-pane label="我，不一樣" name="second">
      <div class="p">
        <pre id="pt1"> 計劃書</pre>
        <img src="../assets/f1.jpg" alt="f1" width="300px" height="400px">
        <img src="../assets/f2.jpg" alt="f2" width="300px" height="400px">
        <img src="../assets/f3.jpg" alt="f3" width="300px" height="400px">
        <img src="../assets/f4.jpg" alt="f4" width="300px" height="400px">
        <pre id="pt3"> 成果展示</pre>
        <img src="../assets/f5.jpg" alt="f5" width="500px" height="350px">
      </div>
    </el-tab-pane>
  </el-tabs>
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
#profile{
  font-family:Arial, Helvetica, sans-serif;
  position: relative;
  top: 95px;
  text-align: center;
  font-size: 72px;
  letter-spacing: 130px;
  color:#DAD7CD;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
}
.op{
  width: 1070px;
  position: relative;
  text-align: center;
  left: 230px;
  top: 150px;
}
.el-tab-pane{
  box-shadow: inset 2px 2px 4px rgba(0, 0, 0, 0.30);
  height: 1600px;
}
.p{
  margin: 50px;
  padding: 50px;
}
.p img{
  position: relative;
  float: center;
  top: 20px;
  left: 0px;
  margin: 10px;
}
#pt1{
  font-family:Arial, Helvetica, sans-serif;
  font-size: 18px;
  color: #DAD7CD;
  letter-spacing: 50px;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
  padding: 30px;
  float: center;
  text-align: center;
}
#pt2{
  font-family:Arial, Helvetica, sans-serif;
  font-size: 18px;
  color: #DAD7CD;
  letter-spacing: 50px;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
  padding: 70px;
  position: relative;
  top: 40px;
  float: center;
  text-align: center;
}
#pt3{
  font-family:Arial, Helvetica, sans-serif;
  font-size: 18px;
  color: #DAD7CD;
  letter-spacing: 50px;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
  padding: 50px;
  position: relative;
  top: 30px;
  float: center;
  text-align: center;
}
#p5{
  padding: 10px;
  position: relative;
  float: center;
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
.el-tabs__item{
height: 60px;
color: #DAD7CD !important;
text-align: center;
padding-top: 10px;
font-size: 18px !important;
font-family:Arial, Helvetica, sans-serif;
text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
font-weight: 600;
}
.is-active{
color:  #A3B18A !important;
text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
font-weight: 600;
}
.el-tabs__active-bar{
  background-color: #A3B18A;
}
</style>

<script>
  export default {
    data() {
      return {
        activeName: 'second'
      };
    },
    methods: {
      handleClick(tab, event) {
        console.log(tab, event);
      }
    }
  };
</script>