<template>
  <div>
    <div class="topcontainer">
      <div class="top-sub-con">
        <div class="blog">
          <div class="wal-h-txt">
            <h1 style="font-size: 60px; float: left; color: white">Nuxt JS</h1>
            <h1 style="font-size: 60px; float: left; color: #00dc82">
              &nbspBlog
            </h1>
          </div>
          <div>
            <p class="wal-para">
              Discover articles from the core team and contributors about
              NuxtJS, tips and tricks included!
            </p>
          </div>
        </div>
        <div class="image-link">
          <a href="https://nuxt.com/">
            <img class="imag" src="img2.png" alt="" />
          </a>
        </div>
      </div>
      <div class="blg-container">
        <!-- <a href=""> -->
        <div class="blg-left-side">
          <div class="blog-heading">
            <h5>Going Full Static</h5>
          </div>
          <div class="blog-desc">
            <p>
              Long awaited features for Jamstack fans has been shipped in v2.13:
              full static build with nuxt export, improved smart prefetching,
              integrated crawler, faster re-deploy, built-in web server and new
              target option for config :zap:️
            </p>
          </div>
          <div class="blog-tags"></div>
          <div class="blog-Author"></div>
        </div>
        <div class="blg-right-side">
          <div class="blg-img"></div>
        </div>
        <!-- </a> -->
      </div>
    </div>
  </div>
</template>

<script></script>

<style>
.topcontainer {
  width: 100%;
  padding-left: 60px;
  padding-right: 60px;
  min-height: 800px;
  color: white;
  background-image: linear-gradient(180deg, #18181b, #323239);
}

.top-sub-con {
  background-color: pink;
  padding-top: 40px;
  height: 420px;
  width: 100%;
}

.blog {
  /* background-color: red; */
  height: 380px;
  padding-top: 40px;
  padding-left: 40px;
  margin-bottom: 100px;
  width: 60%;
  float: left;
}

.image-link {
  /* background-color: blue; */
  width: 35%;
  height: 380px;
  padding-top: 100px;
  float: left;
}
.imag {
  height: 80%;
  width: 100%;
  border-radius: 40px;
}

.wal-para {
  color: white;
  font-size: 20px;
  padding-top: 10px;
  width: 80%;
  padding-bottom: 10px;
  float: left;
}

.blg-container {
  width: 100%;
  height: 500px;
  background-color: red;
}

.blg-left-side {
  /* background-color: blue; */
  float: left;
  width: 65%;
  height: 300px;
}
.blg-right-side {
  float: left;
  height: 300px;
  width: 35%;
  background-color: blue;
}
.blog-heading {
  /* display: flex; */
  width: 100%;
  height: 80px;
  background-color: rgb(182, 26, 52);
  color: white;
}
h5 {
  /* float: left; */
}
.blog-desc {
  background-color: darkred;
  width: 100%;
  height: 110px;
  color: rgba(235, 235, 235, 0.929);
}
.blog-tags {
  background-color: black;
  width: 100%;
  height: 60px;
}
.blog-Author {
  background-color: rgb(177, 56, 56);
  height: 50px;
  width: 100%;
}
</style>
