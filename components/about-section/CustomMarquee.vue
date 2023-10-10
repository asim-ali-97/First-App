<template>
  <div>
    <div class="walppr-txt">
      <div class="wal-h-txt">
        <h1 style="font-size: 60px; float: left; color: white">
          {{ title }} &
        </h1>
        <h1 style="font-size: 60px; float: left; color: #00dc82">
          &nbspexciting Walpapers
        </h1>
      </div>
      <div>
        <p class="wal-para">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Deserunt
          facilis, exercitationem cupiditate cumque esse expedita!
        </p>
      </div>
    </div>
    <div class="marque2">
      <marquee class="marque-div" behavior="" direction="left">
        <div class="sub-marque-div" style="background-image: url('img1.png')">
          <h3>1</h3>
        </div>
        <div class="sub-marque-div" style="background-image: url('img2.png')">
          <h3>2</h3>
        </div>
        <div class="sub-marque-div" style="background-image: url('img3.png')">
          <h3>3</h3>
        </div>
        <div class="sub-marque-div" style="background-image: url('img4.png')">
          <h3>4</h3>
        </div>
      </marquee>
    </div>
  </div>
</template>

<script>
export default {
  name: "CustomMarquee",
  // data() {
  //   return {
  //     title: "About Page",
  //   };
  props: {
    title: {
      type: String,
      default: "",
    },
  },
};
</script>
