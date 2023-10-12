<template>
  <div id="main-cont">
    <div class="top-Bcontainer">
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
      <template v-for="item in blogList">
        <div class="blg-container">
          <a :href="item.blogLink">
            <div class="blg-left-side">
              <div class="blog-heading">
                <h5 class="heding-txt">{{ item.heading }}</h5>
              </div>
              <div class="blog-desc">
                <p>
                  {{ item.desc }}
                </p>
              </div>
              <div class="blog-tags">
                <div class="tag"><p>NUXT</p></div>
                <div class="tag"><p>STATIC</p></div>
                <div class="tag"><p>CRAWLER</p></div>
                <div class="tag"><p>LIVE PREVIEW</p></div>
              </div>
              <div class="blog-Author">
                <div class="auth-img">
                  <img :src="item.image" alt="" />
                </div>
                <div class="auth-name">
                  <h5>{{ item.authName }}</h5>
                </div>
                <div class="date">
                  <ul class="dt-mn">
                    <li>{{ item.pdate }}</li>
                    <li>{{ item.readtime }}</li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="blg-right-side">
              <div class="blg-img"></div>
            </div>
          </a>
        </div>
      </template>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      blogList: [
        {
          heading: "Going Full Static",
          desc: "Long awaited features for Jamstack fans has been shipped Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vitae temporibus mollitia officiis in natus fuga. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vitae temporibus mollitia officiis in natus fuga.",
          image: "dev3.png",
          authName: "Sebastian Chapin",
          pdate: "June 18, 2020",
          readtime: "10 min read",
          blogLink: "https://nuxtjs.ir/blog/going-full-static",
        },
        {
          heading: "Going dark with Nuxtjs color mode",
          desc: "The @nuxtjs/color-mode module is a cool way of adding dark mode to your site.consectetur adipisicing elit. Vitae temporibus mollitia officiis in natus fuga. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vitae temporibus mollitia officiis in natus fuga.",
          image: "dev2.png",
          authName: "Debbie O'Brien",
          pdate: "May 19, 2020",
          readtime: "18 min read",
          blogLink: "https://nuxtjs.ir/blog/going-dark-with-nuxtjs-color-mode",
        },
        {
          heading: "Build a DEV.TO clone with Nuxt new fetch",
          desc: "Let’s build a blazing fast articles and tutorials app using Nuxt, Dev.to API, with lazy loading,.consectetur adipisicing elit. Vitae temporibus mollitia officiis in natus fuga. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vitae temporibus mollitia officiis in natus fuga.",
          image: "dev1.png",
          authName: "Sebastien Chopin",
          pdate: "April 8, 2020",
          readtime: "22 min read",
          blogLink:
            "https://nuxtjs.ir/blog/build-dev-to-clone-with-nuxt-new-fetch",
        },
        {
          heading: "Understanding how fetch works in Nuxt 2.12",
          desc: "Explore different features of the fetch hook and learn a brand new way to bring data into Nuxt applications.",
          image: "dev3.png",
          authName: "Krutie Patel",
          pdate: "April 6, 2020",
          readtime: "17 min read",
          blogLink:
            "https://nuxtjs.ir/blog/understanding-how-fetch-works-in-nuxt-2-12",
        },
        {
          heading: "Introducing Smart Prefeching",
          desc: "Starting from Nuxt v2.4.0, Nuxt.js will automagically prefetch the code-splitted pages linked with a nuxt-link when visible in the viewport by default.",
          image: "dev2.png",
          authName: "Sébastien Chopin",
          pdate: "January 28, 2019",
          readtime: "1 min read",
          blogLink: "https://nuxtjs.ir/blog/introducing-smart-prefetching",
        },
      ],
    };
  },
};
</script>

<style>
.top-Bcontainer {
  width: 100%;
  padding-left: 60px;
  padding-right: 60px;
  height: auto;
  color: white;
  background-image: linear-gradient(180deg, #18181b, #323239);
  padding-bottom: 10px;
}

.top-sub-con {
  /* background-color: pink; */
  padding-top: 40px;
  height: 420px;
  width: 100%;
}

.blog {
  /* background-color: black; */
  height: 380px;
  padding-top: 40px;
  padding-left: 40px;
  width: 60%;
  float: left;
}

.image-link {
  /* background-color: blue; */
  width: 40%;
  padding-left: 20px;
  padding-right: 20px;
  height: 380px;
  padding-top: 100px;
  float: left;
}

@keyframes myshadow {
  50% {
    box-shadow: 10px 20px 30px #00dc82;
  }
}

.imag {
  height: 80%;
  width: 100%;
  border-radius: 40px;
  animation: myshadow 8s infinite;
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
  height: 300px;
  margin-top: 50px;
  margin-bottom: 50px;
  padding-top: 20px;
  padding-left: 20px;
  padding-right: 20px;
  border-radius: 5px;
  background-color: #383845;
  transition: all 0.5s ease 0s;
}
.blg-container:hover {
  background-color: #404050;
  transition: all 0.5s ease 0s;
  .blg-right-side {
    background-color: #383845;
  }
}

.blg-left-side {
  float: left;
  width: 65%;
  height: 260px;
  padding-right: 10px;
}
.blg-right-side {
  float: left;
  height: 260px;
  width: 35%;
  transition: all 0.5s ease 0s;
  /* background-color: green; */
}
.blg-right-side:hover {
  background-color: #383845;
}

.blog-heading {
  width: 100%;
  height: 60px;
  color: white;
}

.heding-txt {
  font-size: 30px;
  width: auto;
  transition: all 0.5s ease 0s;
}
.heding-txt:hover {
  color: #00dc82;
  transition: all 0.5s ease 0s;
}

.blog-desc {
  width: 100%;
  font-weight: 110;
  height: 100px;
  font-size: 18px;
  line-height: 1.3;
  color: rgba(235, 235, 235, 0.815);
}
.blog-tags {
  /* background-color: black; */
  width: 100%;
  height: 60px;
  padding-top: 17px;
}
.tag {
  color: rgba(235, 235, 235, 0.929);
  float: left;
  margin-right: 15px;
  border: 1px solid grey;
  height: 25px;
  padding-left: 6px;
  padding-right: 6px;
  padding-top: 3px;
  border-top-right-radius: 20px;
  border-bottom-right-radius: 20px;
  border-top-left-radius: 20px;
  border-bottom-left-radius: 20px;
}
.tag p {
  font-size: 12px;
}

.blog-Author {
  /* background-color: rgb(177, 56, 56); */
  height: 50px;
  width: 100%;
}
.auth-img {
  float: left;
  height: 30px;
  width: 30px;
  border-radius: 50%;
  overflow: hidden;
}
.auth-img img {
  width: 30px;
  height: 30px;
}

.auth-name {
  padding-top: 5px;
  color: whitesmoke;
  float: left;
  margin-left: 8px;
  /* background-color: blue; */
}
.auth-name h5 {
  font-size: 16px;
  font-weight: 400;
}
.date {
  float: left;
  padding-top: 6px;
  width: 300px;
}
.dt-mn {
  color: rgba(235, 235, 235, 0.929);
  display: flex;
  /* background-color: red; */
}
.dt-mn li {
  font-size: 14px;
  font-weight: 200;
  /* background-color: blue; */
  padding-right: 35px;
}
</style>
