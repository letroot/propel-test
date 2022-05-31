<template>
  <div class="bar-container">
    <!-- TODO: add conditionals for other levels -->
    <div v-if="level === '3'">
      <img class="bar-img" src="../assets/img/kyc-level-3.svg" />
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  level: Number,
});
</script>

<style scoped>
.bar-img {
  width: 50%;
}
</style>
