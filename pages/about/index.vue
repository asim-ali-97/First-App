<template>
  <div id="main-div">
    <div class="top-Acontainer">
      <div class="about">
        <h2 style="font-size: 60px; color: #00dc82">About</h2>
        <p class="wal-para">Welcome to About page</p>
      </div>

      <CustomMarquee title="About page " />
    </div>
  </div>
</template>

<script>
import CustomMarquee from "@/components/about-section/CustomMarquee.vue";
export default {
  components: {
    CustomMarquee,
  },
};
</script>

<style>
.top-Acontainer {
  width: 100%;
  padding-left: 60px;
  height: 800px;
  color: white;
  background-image: linear-gradient(180deg, #18181b, #323239);
}

.about {
  padding-top: 40px;
  padding-left: 40px;
  margin-bottom: 100px;
}

.wal-para {
  color: white;
  font-size: 20px;
  padding-top: 10px;
  width: 80%;
  padding-bottom: 10px;
  float: left;
}

.walppr-txt {
  width: 80%;
  height: 180px;
  padding-left: 60px;
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
