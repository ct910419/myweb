<template>
<div>
	<div class="bg">
    <img src="../assets/bg.png" alt="bg">
  </div>
	<div id="daily">
    <pre> DAILY</pre>
  </div>
	<div class="thr">
		<el-carousel :interval="4000" type="card" height="400px" width="400px">
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="one" src="../assets/1.jpg" alt="1" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="two" src="../assets/2.jpg" alt="2" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="three" src="../assets/3.jpg" alt="3" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="four" src="../assets/4.jpg" alt="4" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="five" src="../assets/5.jpg" alt="5" width="400px" height="400px">
			</el-carousel-item>
  	</el-carousel>
		<div class="t">
			<span>三人行</span>
			<div class="hover">
  		<pre>今年還沒逛到信義區很有耶誕氣氛的那一區
就因為已經2130該回家行程便結束了
好可惜好想再多相處一下
每次見到你們都好開心
你們是什麼充電器吧
和你們聚完我現在的狀態是滿格耶
就好像有動力繼續努力了
-
蜂蜜炸雞好好吃
酷聖石的宇治抹茶也好好吃
結果不小心花了400在吃上面
-
下次見面會是什麼時候呢
我已經開始期待了(ฅ´ω`ฅ)

</pre>
  		</div>
		</div>
	</div>
	<div class="six">
		<el-carousel :interval="4000" type="card" height="400px" width="400px">
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="one" src="../assets/11.jpg" alt="1" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="two" src="../assets/12.jpg" alt="2" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="three" src="../assets/13.jpg" alt="3" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="four" src="../assets/14.jpg" alt="4" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="five" src="../assets/15.jpg" alt="5" width="400px" height="400px">
			</el-carousel-item>
  	</el-carousel>
		<div class="t">
			<span>六人行</span>
			<div class="hover">
  		<pre>這是一個極度荒謬不到兩天的兩日遊
一切不順的開始就是源自於我搭上反方向客運的那一刻
到了台北卻不能回家
還買到一張因為猴硐坍方開車未定的無座票
花了總共5.5小時抵達原本只需要2小時不到的台中
以為衰運到此結束
結果去住宿地點的路上
我們一行人再次搭上了反向公車，離目的地越來越遠
好不容易因為uber新用戶優惠可以去很久沒去的逢甲夜市
甚至是所有人手機都存著我的信用卡卡號
((那你們不要亂刷，我會被line通知我又花錢了
回程的時候優惠被取消
剩下三人差點要騎Ubike回去，回到民宿時已經快12.了
於是旅程的第一天結束
-
第二天是從一場慢手疊杯開始的，還有奇奇怪怪的桌遊
接著就聊天聊天聊天
六個人擠在一張床上，蓋著薄薄寒酸的毯子
其實聊了什麼很多細節我都忘了，只記得木千是渣男
很多高一同學逐漸母湯逐漸歪掉
大家都投二辰一票，但我覺得千層蛋糕很好吃
然後就四點了，早安各位
醒來就已經十點了
發現黃小姐怡瑄昨天把外套放在Ubike的籃子上
於是他花了一小時回逢甲夜市尋找外套，卻還是無功而返
餓了接近16小時，終於找到一間看起來不錯的義大利麵
誰知道我傳了地址給黃小姐，他還是去了另一間分店
之後就去火車站/寄物/坐在廣場玩誰是臥底
朱利亞拜拜/大魯閣不是太魯閣/棒球
音質很爛的唱歌包廂/射飛鏢/投籃機
快樂是10元買得到的/女籃三醜拜拜
莫凡彼的麻糬鬆餅超好吃/同時失戀的兩個女人
想交男友/久大/聖誕節/陳姿佑拜拜/各位寒假見
-
其實也沒幹嘛，但很開心
這大概就是快樂社的宗旨</pre>
  		</div>
		</div>
	</div>
	<div class="ten">
		<el-carousel :interval="4000" type="card" height="400px" width="400px">
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="one" src="../assets/21.jpg" alt="1" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="two" src="../assets/22.jpg" alt="2" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="three" src="../assets/23.jpg" alt="3" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="four" src="../assets/24.jpg" alt="4" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="five" src="../assets/25.jpg" alt="5" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="one" src="../assets/26.jpg" alt="6" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="two" src="../assets/27.jpg" alt="7" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="three" src="../assets/28.jpg" alt="8" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="four" src="../assets/29.jpg" alt="9" width="400px" height="400px">
			</el-carousel-item>
    	<el-carousel-item v-for="item in 1" :key="item" class="pic">
				<img class="item_ig" id="five" src="../assets/30.jpg" alt="10" width="400px" height="400px">
			</el-carousel-item>
  	</el-carousel>
		<div class="t">
			<span>耶舞</span>
			<div class="hover">
  		<pre>20201210
七系聯合耶舞
一個沒有配對
也沒有認識別系
感覺是只有系上耶舞
的耶舞
#藝術學院劍士班</pre>
  		</div>
		</div>
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
#daily{
  font-family:Arial, Helvetica, sans-serif;
  position: relative;
  top: 95px;
  text-align: center;
  font-size: 72px;
  letter-spacing: 195px;
  color:#DAD7CD;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
}
.thr{
	position: relative;
	top: 170px;
	width: 1100px;
	float: center;
	left: 85px;
	background-color: #DAD7CD;
  padding: 100px;
  box-shadow: inset 2px 2px 4px rgba(0, 0, 0, 0.30);
	margin: 10px;
}
.el-carousel__item:nth-child(2n){
  background-color:#dad7cd00;
}
.el-carousel__item:nth-child(2n+1){
  background-color:#dad7cd00;
}
.six{
	position: relative;
	top: 170px;
	width: 1100px;
	float: center;
	left: 85px;
	background-color: #DAD7CD;
  padding: 100px;
  box-shadow: inset 2px 2px 4px rgba(0, 0, 0, 0.30);
	margin: 10px;
}
.ten{
	position: relative;
	top: 170px;
	width: 1100px;
	float: center;
	left: 85px;
	background-color: #DAD7CD;
  padding: 100px;
  box-shadow: inset 2px 2px 4px rgba(0, 0, 0, 0.30);
	margin: 10px;
}
.t{
	font-family: Arial, Helvetica, sans-serif;
	font-size: 20px;
	margin: 20px;
	position: relative;
	float: center;
	top: 30px;
	color:#DAD7CD;
  background-color: #DAD7CD;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
	letter-spacing: 20px;
}
.t:hover .hover{
  display:block;
}
.hover{
  display:none;
	position: relative;
	float: center;
	top: 20px;
	font-size: 16px;
	line-height: 40px;
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
