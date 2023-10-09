<template>
  <div>
    <nav class="nav">
      <div class="nav-left">
        <div class="logo">
          <img src="logo.svg" alt="">
        </div>
      </div>
      <div class="header">
        <div @click="$router.push('/')" class="header-item">Home</div>
        <div @click="$router.push('/about')" class="header-item">About Us</div>
        <div @click="$router.push('/contact')" class="header-item">Contact</div>
        <div @click="$router.push('/blog')" class="header-item">Blog</div>
      </div>
      <div class="nav-right">
        <div class="icon">
          <img class="git" src="github-line.svg" height="27px" width="27px" alt="">
        </div>
      </div>
    </nav>


  </div>
</template>
  
<script>

</script>
  
<style>
.nav {
  width: 100%;
  height: 80px;
  background-color: #18181B;
}
.icon{
  margin-right: 40px;
  margin-top: 20px;
  float: right;
  border-radius: 50%;
  height: 30px;
  width: 30px;
  background-color: #fff;
}
.git{
  margin-left: 1px;
  border-radius: 50%;
}

.nav-left {
  padding-left: 25px;
  /* line-height: 80px; */
  padding-top: 20px;
  width: 33.3%;
}

.header {
  padding-left: 25px;
  width: 33.4%;
  line-height: 80px;
}

.header-item {
  float: left;
  color: white;
  padding-left: 25px;
  padding-right: 25px;
}

.nav-right {
  color: white;
  width: 33.3%;
}

.header-item:hover {
  background-color: #515157;
}
</style>