<template>
  <div>
    <Nav />
    <div class="container">
      <SideBar />
      <div class="kyc-container">
        <KYCProgressBar level="3" />
        <AddPhotoKYC />
      </div>
    </div>
  </div>
</template>

<script setup>
import SideBar from "./SideBar.vue";
import Nav from "./GlobalNav.vue";
import KYCProgressBar from "./KYCProgressBar.vue";
import AddPhotoKYC from "./AddPhotoKYC.vue";
</script>

<style scoped>
@import "../assets/css/base.css";

.container {
  height: 100vh;
  display: flex;
}

.kyc-container {
  display: flex;
  flex-direction: column;
  margin: auto;
  margin-top: 15vh;
  width: 
}
</style>
