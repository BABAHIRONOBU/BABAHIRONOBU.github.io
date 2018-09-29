<template>
  <view-port row position align-center justify-center>
    <div class="background-left"></div>
    <div class="background-right"></div>
    <div class="profile">
      <div class="name"></div>
      <div class="occupation"></div>
      <div class="profile-image-wrapper">
        <img class="profile-image" src="" alt="">
      </div>
      <div class="info">
        <div class="birth"></div>
        <div class="email"></div>
        <div class="short-message"></div>
      </div>
    </div>
  </view-port>
</template>

<script>
import ViewPort from '../components/ViewPort.vue'

export default {
  components: { ViewPort }
}
</script>

<style>
/* .view-port {
  height: 100vh;
  display: flex;
  position: relative;
  align-items: center;
  justify-content: center;
} */
.background-left {
  position: absolute;
  left: 0;
  height: 100%;
  width: 42.8571%;
  z-index: -1;
  background-color: #f1c232ff;
  border-right: 5px solid black;
}
.background-right {
  position: absolute;
  right: 0;
  height: 100%;
  width: 57.1429%;
  z-index: -1;
  background-color: #01afd1ff;
  border-left: 5px solid black;
}
.profile {
  width: 718px;
  height: 650px;
  background-color: white;
  border: 1px solid black;
}
</style>
