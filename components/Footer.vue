<template>
  <div>
    <footer class="footer">
      <div class="footr-left">
        <div>
          <ul>
            <li>Hope you find it Useful</li>
            <li>Hope can we help you?</li>
            <li>FAQ's</li>
          </ul>
        </div>
      </div>

      <div class="footer-middle">
        <div @click="$router.push('/')" class="footer-item">Home</div>
        <div @click="$router.push('/about')" class="footer-item">About Us</div>
        <div @click="$router.push('/contact')" class="footer-item">Contact</div>
        <div @click="$router.push('/blog')" class="footer-item">Blog</div>
      </div>

      <div class="footr-right">
        <div class="right-ftr-item">
          <h6>Reach out us on</h6>
          <a href="https://www.facebook.com/">Facebook</a><br />
          <a href="https://www.instagram.com/">Instagram</a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script></script>

<style>
.footer {
  color: white;
  width: 100%;
  height: 100px;
  background-color: #18181b;
}

.footr-left {
  width: 33.3%;
  height: 100px;
  padding-top: 15px;
  padding-left: 25px;
  float: left;
}

.footer-middle {
  width: 33.3%;
  line-height: 100px;
  float: left;
}

.footer-item {
  padding-left: 30px;
  padding-right: 30px;
  float: left;
}

.footer-item:hover {
  color: #00dc82;
}

.footr-right {
  height: 100px;
  width: 33.3%;
  padding-top: 15px;
  padding-right: 5px;
  float: left;
  color: white;
}
.right-ftr-item {
  padding-left: 100px;
}
a {
  color: white;
}
</style>
