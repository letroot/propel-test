<template>
  <div>
    <nav>
      <div class="nav-items">
        <img src="../assets/img/logo.svg" alt="Propel logo in black" />
      </div>
    </nav>
  </div>
</template>

<script setup></script>

<style scoped>
@import "../assets/css/base.css";

nav {
  display: flex;
  padding: 42px 0;
  align-items: center;
  height: 10vh;
  background-color: transparent;
  position: fixed;
  z-index: 42;
}

nav .nav-items {
  margin-left: 8vw;
}

nav .nav-items img {
  height: 36px;
}
</style>
