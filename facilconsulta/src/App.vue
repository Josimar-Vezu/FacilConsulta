<template>
  <div>
    <nav class="painelnav">
      <ul>
        <li id="homebuttom"><a href="/#/" id="textbuttom">HOME</a></li>
      </ul>
    </nav>
    <router-view></router-view>
  </div>
</template>


<script>
export default {};
</script>

<style>
html,
body {
  margin: 0 auto;
  background-color: #ffe766;
}

.painelnav {
}

#homebuttom {
  width: 350px;
  height: 50px;
  border-radius: 15px;
  display: block;
  margin: 25px;
  background-color: #483698;
}

#textbuttom {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  color: white;
  -webkit-font-smoothing: antialiased;
  margin: 25px;
  text-align: center;
  margin-top: 1200px;
  margin-left: 140px;
}
</style>