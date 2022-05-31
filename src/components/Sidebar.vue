<template>
  <div>
    <aside class="side-bar">
      <div class="footer">
        <ul>
          <li :key="index" v-for="(value, key, index) in footerLinks">
            <a :href="value">{{ key }}</a>
          </li>
        </ul>
      </div>
    </aside>
  </div>
</template>

<script setup>
const footerLinks = {
  "©Propel, 2022": "#",
  "Privacy policy": "#",
  "Contact us": "#",
  "Terms of use": "#",
};
</script>

<style scoped>
@import "../assets/css/base.css";

aside.side-bar {
  width: 35vw;
  height: 100vh;
  background-color: var(--orange-50);
  display: flex;
  flex-direction: column;
}

aside .footer {
  margin-top: auto;
  margin-left: 8vw;
  margin-bottom: 1rem;
  font-size: var(--text-xs);
}

aside .footer ul {
  font-size: var(--text-xs);
  list-style: none;
  display: flex;
  gap: 24px;
}

aside .footer ul a {
  color: var(--gray-200);
  text-decoration: underline;
  text-underline-position: under;
}
</style>
