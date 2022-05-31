<template>
  <div>
    <div class="apk-container">
      <header>
        <h3>Add a profile photo</h3>
        <p>
          Before you continue, please take a moment to <br />
          complete your profile
        </p>
      </header>
      <div class="widget-container">
        <img
          @click="uploadPhoto"
          src="../assets/img/upload-photo.svg"
          alt="upload photo button"
        />
      </div>
      <div class="btn-container">
        <button class="primary-btn back-btn">Back</button>
        <button class="primary-btn cta-btn">Save & continue</button>
      </div>
    </div>
  </div>
</template>

<script setup>
function uploadPhoto() {
  // do something neat
}
</script>

<style scoped>
@import "../assets/css/base.css";

.apk-container {
  display: flex;
  flex-direction: column;
  height: auto;
  margin-top: 28px;
}

h3 {
  font-size: var(--text-h3);
  font-family: Gilroy, sans-serif;
  font-weight: bold;
}

p {
  color: var(--gray-200);
  font-size: var(--text-sm);
}

.widget-container {
  text-align: center;
}

.widget-container img {
  width: 180px;
  margin-top: 28px;
  /* margin: auto 0; */
}

.btn-container {
  display: flex;
  justify-content: space-between;
  margin-top: 75px;
}

.primary-btn {
  border-radius: var(--border-btn);
  border: none;
  font-weight: bold;
  font-size: 12px;
}

.back-btn {
  padding: 10px 15px;
  border-radius: 8px;
  background-color: var(--orange-50);
  color: var(--gray-200);
}

.back-btn:hover {
  background-color: var(--orange-60);
}

.cta-btn {
  background-color: var(--cta-blue);
  color: white;
  border-radius: 9px;
  padding: 8px 12px;
}
</style>
