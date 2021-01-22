<template>
<div>
  <div id="app">
    <div id="nav">
      <router-link to="/" id="w">Home&nbsp;&nbsp;</router-link>
      <router-link to="/about" id="w">About&nbsp;&nbsp;</router-link>
      <router-link to="/profile" id="w">Profile&nbsp;&nbsp;</router-link>
      <router-link to="/daily" id="w">Daily&nbsp;&nbsp;</router-link>
      <router-link to="/game" id="w">Funny&nbsp;&nbsp;</router-link>
    </div>
    <router-view/>
  </div>
</div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  z-index: 999;
}
#nav{
  position: sticky;
  left: 0;
  margin: 20px;
}
#nav a{
  font-weight: bold;
  text-decoration:none;
  font-size: 25px;
  box-shadow:4px 2px 4px rgba(0, 0, 0, 0.30);
}
#w{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: #DAD7CD;
  padding: 20px;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
  margin: 20px;
}
#nav a.router-link-exact-active {
  color: #A3B18A;
  text-shadow: rgba(255, 255, 255, 0.1) -2px -2px 1px, rgba(0, 0, 0, 0.5) 1px 1px 1px;
  font-size: 25px;
}
</style>