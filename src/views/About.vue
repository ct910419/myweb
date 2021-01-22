<template>
<div>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>
<template>
<div>
  <div class="bg">
    <img src="../assets/bg.png" alt="bg">
  </div>
  <div id="about">
    <pre> ABOUT</pre>
  </div>
  <div id="tseng">
    <pre class="swingHorizontal">夏綠蒂曾</pre>
  </div>
  <div id="text">
    <pre class="swingHorizontal">2002.04 三軍總醫院出生
2008.08 畢業於忠孝托兒所
2013.02 北市花式直排輪高年級組第一
2013.09 加入興雅國樂團
2014.06 畢業於興雅國小
2014.08 圍棋初段
2015.08 鋼琴7級檢定
2017.06 畢業於介壽國中
2017.09 加入合唱團
2018.12 校內詩歌朗誦佳作
2019.04 校內國語朗讀優等
2020.06 畢業於松山高中
2020.09 就讀清華大學藝術學院學士班
.
.
.</pre>
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
#about{
  font-family:Arial, Helvetica, sans-serif;
  position: relative;
  top: 95px;
  text-align: center;
  font-size: 72px;
  letter-spacing: 195px;
  color:#DAD7CD;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
}
.me{
  position: relative;
  top: 180px;
  float: left;
  left: 593px;
  box-shadow:4px 2px 4px rgba(0, 0, 0, 0.30);
}
.me img{
  width: 255px;
  height: 281px;
}
#tseng{
  font-size: 25px;
  letter-spacing: 53px;
  position: absolute;
  top: 454px;
  float: left;
  text-align: left;
  left: 280px;
  font-family: Arial, Helvetica, sans-serif;
  font-weight: 600;
  color: #A3B18A;
  text-shadow: rgba(255, 255, 255, 0.1) -1px -0.5px 8px, rgba(0, 0, 0, 0.5) 1px 1px 0px;
}
#text{
  font-size: 22px;
  letter-spacing: 23px;
  position: absolute;
  float: center;
  text-align: left;
  top: 550px;
  left: 280px;
  line-height: 100px;
  font-weight: 600;
  color: #A3B18A;
  text-shadow: rgba(255, 255, 255, 0.1) -1px -0.5px 8px, rgba(0, 0, 0, 0.5) 1px 1px 0px;
}
.swingHorizontal{
    color: #A3B18A;
}

.swingHorizontal:hover
{
    animation: swingHorizontal 1s ease;
    animation-iteration-count: 5;
}

@keyframes swingHorizontal
{
    15%
    {
        transform: translateX(5px);
    }
    30%
    {
        transform: translateX(-5px);
    }
    50%
    {
        transform: translateX(3px);
    }
    65%
    {
        transform: translateX(-3px);
    }
    80%
    {
        transform: translateX(2px);
    }
    100%
    {
        transform: translateX(0);
    }
}
</style>
