<template>
  <div id="main-div">
    <div class="topcontainer">
      <div class="topsubcon">
        <h2>The Intuitive Web Framework</h2>
        <p class="top-para">
          Welcome to home page Lorem ipsum dolor. Quibusdam amet alias suscipit
          at molestias, inventore delectus, temporibus nesciunt sapiente beatae
          pariatur nostrum.
        </p>
        <div class="button-blg">
          <CustomPrimaryBtn
            @click="$router.push('/blog')"
            title="Read our Blogs"
          />
        </div>
      </div>
      <div class="topsubcon"></div>
    </div>

    <div class="walppr-txt">
      <div class="wal-h-txt">
        <h1 style="font-size: 60px; float: left; color: white">Our Team of</h1>
        <h1 style="font-size: 60px; float: left; color: #00dc82">
          &nbspDevelopers
        </h1>
      </div>
      <div>
        <p class="wal-para">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Deserunt
          facilis, exercitationem cupiditate cumque esse expedita!
        </p>
      </div>
    </div>

    <div class="dev-sec">
      <template v-for="item in userList">
        <div class="dev-sub-sec">
          <img class="dev-img" :src="item.image" />
          <div class="dev-name">
            <h4>{{ item.name }}</h4>
          </div>
          <div class="dev-info">
            <p>
              {{ item.desc }}
            </p>
          </div>
        </div>
      </template>
    </div>

    <!-- props -->
    <CustomMarquee />
  </div>
</template>

<script>
import CustomPrimaryBtn from "@/components/CustomPrimaryBtn.vue";
import CustomMarquee from "@/components/about-section/CustomMarquee.vue";
export default {
  components: {
    CustomPrimaryBtn,
    CustomMarquee,
  },
  data() {
    return {
      userList: [
        {
          name: "Shakil Ahmad",
          desc: "sak Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores laborum dolorum iste ex ab. Exercitationem.",
          image: "dev1.png",
        },
        {
          name: "Asim Ali",
          desc: "asm Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores laborum dolorum iste ex ab. Exercitationem.",
          image: "dev2.png",
        },
        {
          name: "Muhib Arsalan",
          desc: "mhb Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores laborum dolorum iste ex ab. Exercitationem.",
          image: "dev3.png",
        },
      ],
    };
  },
};
</script>

<style>
#main-div {
  background-color: #323239;
}

.topcontainer {
  width: 100%;
  padding-left: 60px;
  height: 700px;
  color: white;
  background-image: linear-gradient(180deg, #18181b, #323239);
}

.topsubcon {
  width: 50%;
  padding-top: 160px;
}

h2 {
  font-size: 80px;
  font-weight: 500;
}

.top-para {
  color: white;
  font-size: 20px;
  padding-top: 10px;
  width: 80%;
  padding-bottom: 10px;
}
.wal-para {
  color: white;
  font-size: 20px;
  padding-top: 10px;
  width: 80%;
  padding-bottom: 10px;
  float: left;
}

.button-blg {
  margin-top: 20px;
}

.walppr-txt {
  width: 80%;
  height: 180px;
  padding-left: 60px;
}

.dev-sec {
  width: 90%;
  margin-left: 5%;
  margin-top: 20px;
  margin-bottom: 150px;
  height: 350px;
  display: flex;
  justify-content: space-between;
}

.dev-sub-sec {
  width: 32%;
  height: 350px;
  border-radius: 10px;
  background-color: #4b4b4f;
  overflow: hidden;
  color: white;
}
.dev-sub-sec:hover {
  border: 3px solid #e5e7eb;
}

.dev-img {
  border-radius: 10px;
  width: 100%;
  height: 210px;
  background-repeat: no-repeat;
  background-size: 100% 210px;
}
.dev-name {
  padding-top: 10px;
  padding-left: 20px;
  height: 50px;
}
.dev-info {
  padding-left: 20px;
}

.marque2 {
  margin-left: 5%;
  width: 90%;
  height: 170px;
  border-top-right-radius: 10px;
  border-top-left-radius: 10px;
  overflow: hidden;
}

.sub-marque-div {
  float: left;
  margin-left: 20px;
  width: 250px;
  height: 150px;
  color: white;
  padding-left: 120px;
  padding-top: 110px;
  border-radius: 10px;
}
</style>
